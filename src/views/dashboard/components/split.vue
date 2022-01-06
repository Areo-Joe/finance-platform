<template>
    <div id="split-div">
        <div class="header">
            <h1>FICAS——</h1>
            <h1>金融信息收集分析展示平台</h1>
        </div>
        <div class="entry-container">
            <div id="entry1" class="entry">
                <el-card :body-style="{ padding: '0px' }">
                    <div class="flex-container">
                        <div class="p-div">
                            <img src="../../../assets/1.jpg" class="image">
                        </div>
                        <div style="padding: 14px;text-align:center" class="elb-div">
                            <span>财经要闻</span>
                            <div class="bottom clearfix" style="margin-top: 20px">
                                <el-button type="primary" class="button">News</el-button>
                            </div>
                        </div>
                    </div>
                </el-card>
            </div>
            <div id="entry2" class="entry">
                <el-card :body-style="{ padding: '0px' }">
                    <div class="flex-container">
                        <div class="p-div">
                            <img src="../../../assets/2.jpg" class="image">
                        </div>
                        <div style="padding: 14px;text-align:center" class="elb-div">
                            <span>上市公司财务信息</span>
                            <div class="bottom clearfix" style="margin-top: 20px">
                                <el-button type="primary" class="button">Infomation</el-button>
                            </div>
                        </div>
                    </div>
                </el-card>
            </div>
            <div id="entry3" class="entry">
                <el-card :body-style="{ padding: '0px' }">
                    <div class="flex-container">
                        <div class="p-div">
                            <img src="../../../assets/3.jpg" class="image">
                        </div>
                        <div style="padding: 14px;text-align:center" class="elb-div">
                            <span>股票行情</span>
                            <div class="bottom clearfix" style="margin-top: 20px">
                                <el-button type="primary" class="button">Market</el-button>
                            </div>
                        </div>
                    </div>
                </el-card>
            </div>
            <div id="entry4" class="entry">
                <el-card :body-style="{ padding: '0px' }">
                    <div class="flex-container">
                        <div class="p-div">
                            <img src="../../../assets/量化交易.jpg" class="image">
                        </div>
                        <div style="padding: 14px;text-align:center" class="elb-div">
                            <span>量化交易股票推荐</span>
                            <div class="bottom clearfix" style="margin-top: 20px">
                                <el-button type="primary" class="button">Recommended</el-button>
                            </div>
                        </div>
                    </div>
                </el-card>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.flex-container {
    height: 375px;
    display: grid;
    grid-template-rows: 50% 50%;
}
.el-card {
    height: 100%;
}
img {
    width: 100%;
}
#split-div {
    min-height: calc(90vh - 50px);
    display: grid;
    grid-template-rows: 30% 70%;
    height: 100%;
    .header {
        grid-row: 1 / 2;
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;
        text-align: center;
        h1:nth-child(1) {
            position: relative;
            right: 220px;
        }
        h1 {
            color: rgb(22, 6, 61);
        }
    }
    .entry-container {
        grid-row: 2 / 3;
        border-bottom-left-radius: 5px;
        border-bottom-right-radius: 5px;
        display: grid;
        grid-template-columns: 25% 25% 25% 25%;
        column-gap: 20px;
        #entry1 {
            grid-column: 1 / 2;
            border-bottom-left-radius: 5px;

        }
        #entry2 {
            grid-column: 2 / 3;
        }
        #entry3 {
            grid-column: 3 / 4;
        }
        #entry4 {
            grid-column: 4 / 5;
            border-bottom-right-radius: 5px;
        }
        .entry {
            border-radius: 5px;
            box-shadow: 0 0 5px whitesmoke;
            display: flex;
            flex-direction: column;
            background-color: rgba(84, 170, 250, 0.24);
            .p-div {
                grid-row: 1 / 2;
                overflow: hidden;
            }
            .elb-div {
                grid-row: 2 / 3;
                text-align: center;
            }
        }
    }
}
</style>