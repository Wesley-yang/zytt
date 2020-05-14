<template>
	<view class="content">
		<zyflow :flowlist="datalist" @flowtap="touchcard" @flowget="adddata" ></zyflow>
	</view>
</template>

<script>
	// 导入瀑布流组件
	import zyflow from "../../components/zyflow/zyflow.vue";
	export default {
		//注册组件
		components:{
			zyflow
		},
		data() {
			return {
				datalist:[
					{
						src:"../../static/4.jpg",
						title:'江南可采莲,莲叶何田田.鱼戏莲叶间.鱼戏莲叶东,鱼戏莲叶西,鱼戏莲叶南,鱼戏莲叶北',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:true,
						text:'限时促销小助手为您推荐'
					},
					{
						src:"../../static/2.jpg",
						title:'北朝民歌 敕勒川,阴山下.天似穹庐,笼盖四野.天苍苍,野茫茫,风吹草低见牛羊',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:true,
						text:'您浏览过的足迹'
					},
					{
						src:"../../static/3.jpg",
						title:'鹅,鹅,鹅,曲项向天歌,白毛浮绿水,红掌拨清波',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'限时促销小助手为您推荐'
					},
					{
						src:"../../static/1.jpg",
						title:'解落三秋叶,能开二月花.过江千尺浪,入竹万竿斜',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'您浏览过的足迹'
					},	{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'碧玉妆成一树高,万条垂下绿丝绦.不知细叶谁裁出,二月春风似剪刀',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'限时促销小助手为您推荐'
					},
					{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'黄河远上白云间,一片孤城万仞山,羌笛何须怨杨柳,春风不度玉门关',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'您浏览过的足迹'
					},
					{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'春眠不觉晓,处处闻啼鸟.夜来风雨声,花落知多少',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'限时促销小助手为您推荐'
					},
					{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'寒雨连江夜入吴,平明送客楚山孤.洛阳亲友如相问,一片冰心在玉壶',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'限时促销小助手为您推荐'
					}
				]
			}
		},
		onLoad() {
			
		},
		methods: {
			touchcard(e){
				console.log('点击此项获取到的数据')
				console.log(e);	
			},
			adddata(){
				console.log('调用增加数据函数');
				this.datalist = this.datalist.concat([{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'春眠不觉晓,处处闻啼鸟.夜来风雨声,花落知多少',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'您浏览过的足迹'
					},
					{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'寒雨连江夜入吴,平明送客楚山孤.洛阳亲友如相问,一片冰心在玉壶',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'限时促销小助手为您推荐'
					},{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'春眠不觉晓,处处闻啼鸟.夜来风雨声,花落知多少',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'您浏览过的足迹'
					},
					{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'寒雨连江夜入吴,平明送客楚山孤.洛阳亲友如相问,一片冰心在玉壶',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'限时促销小助手为您推荐'
					},{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'春眠不觉晓,处处闻啼鸟.夜来风雨声,花落知多少',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'您浏览过的足迹'
					},
					{
						src:"../../static/"+Math.floor(Math.random()*4+1)+".jpg",
						title:'寒雨连江夜入吴,平明送客楚山孤.洛阳亲友如相问,一片冰心在玉壶',
						orig:Math.floor(Math.random()*1000),
						money:Math.floor(Math.random()*1000),
						showText:Math.floor(Math.random()+0.5)==1?true:false,
						text:'限时促销小助手为您推荐'
					}])
			}
		}
	}
</script>

<style>
	.content {
		width: 100%;
		height: 100%;
		position: absolute;
		background-color: #bfa;
	}
</style>
