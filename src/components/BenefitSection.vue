<template>
    <div class="section-wrapper benefit">
        <Title></Title>
        <div class="container">
            <div class="row">
                <div class="col-sm-6">
                    <span class="image"> <img src="@/assets/images/left-image.png"></span>
                </div>

                <div class="col-sm-6">
                    <ul class="benlist">
                        <li>
                            <span class="number">
                                1
                            </span>
                            <div class="desc">
                                <h3>Increased flexibility</h3>
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Quisque efficitur vestibulum imperdiet. Vivamus ac
felis mattis, sagittis lectus at, mollis turpis.</p>
                            </div>
                        </li>
                        <li>
                            <span class="number">
                                2
                            </span>
                            <div class="desc">
                                <h3>Increased muscle strength and tone</h3>
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Quisque efficitur vestibulum imperdiet. Vivamus ac
felis mattis, sagittis lectus at, mollis turpis.</p>
                            </div>
                        </li>
                        <li>
                            <span class="number">
                                3
                            </span>
                            <div class="desc">
                                <h3>Improved respiration, energy and vitality</h3>
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Quisque efficitur vestibulum imperdiet. Vivamus ac
felis mattis, sagittis lectus at, mollis turpis.</p>
                            </div>
                        </li>
                        <li>
                            <span class="number">
                                4
                            </span>
                            <div class="desc">
                                <h3>Maintaining a balanced metabolism</h3>
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.
Quisque efficitur vestibulum imperdiet. Vivamus ac
felis mattis, sagittis lectus at, mollis turpis.</p>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import Title from '@/components/Title.vue'
export default {
    name: 'BenefitSection',
    components: {
        Title
    }
}
</script>
<style lang="scss">
.benefit {
    position: relative;
    &:after{
        content: '';
        width: 104%;
        background: #f1f0f0;
        height: 130%;
        position: absolute;
        top: 0;
        left: -50%;
        border-radius: 100%;
        z-index: -1;
    }
    .image {
        width: 100%;
        position: absolute;
        bottom: 0;
        top: 0;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .benlist {
        text-align: left;
        li {
            display: flex;
            align-items: flex-start;
            padding-bottom: 15px;
            .number {
                padding-right: 20px;
            }
            h3 {
                font-weight: 500;
                font-size: 20px;
            }
            p {
                font-size: 16px;
                color: #A39B9B;
                font-weight: normal;
            }
        }
    }
}

</style>