<template>
    <div class="section-wrapper footer">
        <div class="container">
            <div class="row">
                <div class="subscribe">
                    <h5>Get an update from us</h5>
                    <form class="form-inline">
                        <div class="form-group mx-sm-3 mb-2">
                            <label for="inputPassword2" class="sr-only">Password</label>
                            <input type="text" class="form-control" id="inputEmail" placeholder="Email">
                        </div>
                        <button type="submit" class="btn btn-primary mb-2">SUBSCRIBE</button>
                    </form>
                </div>
                <div class="bottom-wrapper">
                    <span class="copyright">
                        <p>Copyright 2020 | Melu Yoga</p>
                    </span>
                    <span class="socials">
                        <ul>
                            <li>
                                facebook
                                <i class="fa fa-facebook"></i>
                            </li>
                            <li>
                                instagram
                                <i class="fa fa-facebook"></i>
                            </li>
                            <li>
                                twitter
                                <i class="fa fa-facebook"></i>
                            </li>
                            <li>
                                youtube
                                <i class="fa fa-facebook"></i>
                            </li>
                        </ul>
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Footer'
}
</script>
<style lang="scss">
.footer {
    background: #333333;
    color: #ffffff;
    .subscribe {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 100%;
        h5{
            color: #ffffff;
        }
    }
    .bottom-wrapper {
        display: flex;
        width: 100%;
        padding-top: 30px;
        margin-top: 30px;
        border-top: 1px solid #ffffff;
        .socials {
            margin-left: auto;
             ul {
                display: flex;
                li {
                    padding-left: 10px;
                }
            }
        }
    }
}

</style>