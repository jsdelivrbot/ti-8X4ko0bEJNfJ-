<template>
    <header class="row header clearfix" style="position:relative;">
        <div class="pull-left pad0 w315">
            <ul class="clearfix" id="">
                <li class="pull-left wb50 text-left"><img src='/lib/img/public/logo.png' class="logo mt5 ml35"/></li>
                <li class="pull-left wb40" id="logo_icon">
                    <p class="text-center fc-fff fs18 mt10">生产管理系统</p>
                    <p class="text-center fc-fff f12">当前版本2.0</p>
                </li>
            </ul>
        </div>
        <div class="fc-fff pad0 f16" style="padding-top:18px;overflow:hidden;">
            <span class="mr35"><a href="#/productioncontrol">种植管理</a></span>
            <span class="mr35"><a href="#/worker/workerorder/workerorder_list">工人管理</a></span>
            <span class="mr35"><a href="#/materialmanagement">物料管理</a></span>
            <span class="mr35"><a href="#/worker/production/production_sum">生产汇总表</a></span>
            <span class="mr35">消息</span>
            <span class=""><a href="#/Home">基础设置</a></span>
        </div>
        <div class="pad0 w415 pull-right" style="position:absolute;top:0;right:10px;">
            <p class="text-right fc-fff">
                <i class="icon-angle-left f16 ml15"></i>
                <i class="icon-angle-right f16 ml15"></i>
                <i class="glyphicon glyphicon-repeat f14 ml15"></i>
                <span class="f14 ml15">提交反馈</span>
                <span class="f14 ml15">使用帮助</span>
                <span class="f14 ml15">摩登庄园</span>
                <i class="icon-minus f14 ml10"></i>
                <i class="icon-check-empty f14 ml10"></i>
                <i class=" icon-remove f14 ml10 mr10"></i>
            </p>
            <p class="text-right fc-fff">
                <i class="fa fa-user-o mr10"></i>
                <span class="mr10">{{worker_name}}</span>
                <span class="mr10">{{role_name}}</span>
                <span class="mr10" v-if="role_id != 1">{{group_name}}</span>
                <i class="icon-caret-down mr10 mt5"></i>
            </p>
        </div>
    </header>
</template>

<script>
	export default {
        name: 'top',
        data:function(){
            return{
                worker_name: localStorage.getItem('worker_name'),
                role_name: localStorage.getItem('role_name'),
                role_id: localStorage.getItem('role_id')
            }
        },
		mounted: function() {

		}
	}

</script>
<script>

</script>
<style scoped>


</style>
