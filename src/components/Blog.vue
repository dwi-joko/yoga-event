<template>
    <div class="section-wrapper blogs">
        <Title></Title>
        <div class="container">
            <div class="row">
                <div v-for="blogs in blogs" :key="blogs.id"  class="col-sm-4 col-xs-12">
                    <div class="blog-item">
                        <span class="images"> <img :src="blogs.image"> </span>
                        <h3>{{ blogs.title }}</h3>
                        <div class="desc">
                            <ul>
                                <li>
                                    <span class="icon">1</span>
                                    <span class="text">5 June 2019</span>
                                </li>
                                <li>
                                    <span class="icon">2</span>
                                    <span class="text">By {{blogs.author}}</span>
                                </li>
                                <li>
                                    <span class="icon">3</span>
                                    <span class="text">3 Likes</span>
                                </li>
                            </ul>
                        </div>
                        <div class="text-blog">
                            <p>{{ blogs.content }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <button class="btn btn-outline tosca">LOAD MORE</button>
    </div>
</template>
<script>
import axios from 'axios'
import Title from '@/components/Title.vue'

export default {
    name: 'Blog',
    components:{
        Title
    },
    data(){
    return {
      blogs : []

    }
  },
  async mounted(){

    this.load()

  },

  methods: {

    async load(){

      const response = await axios.get('http://localhost:3000/blogs')
      this.blogs = response.data

    },

    async save() {
        const response = await axios.post('http://localhost:3000/blogs', this.form)
        this.blogs = response.data
        this.author=''
        this.image=''
        this.title =''
        this.content =''
        this.load()
      } 


  }


}
</script>

<style lang="scss">
    .blogs{
        .blog-item {
            text-align: left;
            padding: 15px;
            border: 1px solid #eaeaea;
            .images{
                width: 100%;
                display: block;
                padding-bottom: 15px;
                img{
                    width: 100%;
                }
            }
            h3 {
                min-height: 70px;
            }
            .desc {
                ul {
                    padding: 0;
                    li {
                        display: inline-block;
                        padding-right: 10px;
                        span {
                            font-size: 12px;
                        }
                        .icon {
                            padding-right: 5px;
                        }
                    }
                }
            }
            p {
                max-height: 75px;
                overflow: hidden;
            }
        }
        button{
            margin-top: 30px;
        }
    }

</style>