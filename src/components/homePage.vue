<template>
	<div class="homePage">
		<!-- 头部部分 -->
		<div class="homebg">
			<!-- 背景图 -->
			<img src="./img/bg1.png" alt="" class="homeTitlebg">
			<img src="./img/titleName.png" alt="" class="homeText">
			<!-- 单位 -->
			<div class="unit">
				<span>指导单位：前海管理局</span>
				<span>主办单位：前海科创投控股有限公司</span>
				<span>承办单位：前海深港青年梦工场&ensp;第一路演</span>
				<img src="./img/LOGO@2x.png" alt="" style="height:20px;width:auto;margin-top:2px">
			</div>
			<div class="icon-video transform"></div>
			<audio src="https://static.dyly.com/h5/h5style/jinghe/bg.mp3" id="bg-music" controls="controls" autoplay="autoplay"
				loop></audio>
		</div>
		<div class="homeBody">
			<div class="headlineleft" style="width:73.6%;">· 活动背景 ·</div>
			<div class="activityBg" style="margin-bottom:50px;">
				粤港澳大湾区建设是习近平总书记亲自谋划、亲自部署、亲自推动的国家战略，是新时代推动形成全面开放新格局的新尝试，是推动“一国两制”事业发展的新实践，也是前海新时期开发开放重大战略机遇。前海立足国家战略优势，汇聚全球创新能量，建设“一带一路”国际路演中心，为全球科技创新企业提供资本及产业资源支持，搭建路演展示舞台，推动粤港澳大湾区建设。
			</div>
			<div class="headlineright" style="width:89.3%;">· 巴西-葡萄牙科创企业专场路演 ·</div>
			<div class="activityBg" style="margin-bottom:50px;clear:both;margin-bottom:55px;">
				本次活动由“一带一路”前海国际路演中心携手澳门经济局产业发展厅，共同邀请巴西及葡萄牙孵化中心及在孵的科创企业来深，包括大数据、云计算、人工智能、物联网、海洋经济、大健康等领域16个深具发展潜力的创新科技项目进行路演，本次路演特邀产业专家、资深投资人组成的评委嘉宾团与路演企业深入沟通，以及众多粤港澳及海外投资机构与会深度点评互动。
			</div>
			<div class="headlineleft" style="width:73.6%;">
				· 活动流程 ·
			</div>
			<!-- 时间轴 -->
			<div class="timeShaft">
				<img src="./img/timeshift.png" alt="" class="timeShiftimg">
			</div>
			<!-- 路演项目 -->
			<div class="headlineright" style="width:73.6%;margin-top:10px;margin-bottom:19px">
				· 路演项目 ·
			</div>
			<!-- 路演项目列表 -->
			<div class="projectItemList">
				<img src="./img/projectItem.png" alt="">
			</div>
			<!-- 嘉宾评委团 -->
			<div class="headlineleft" style="width:75%;margin-top:52px;display:flex;align-items:center">
				· 嘉宾评委团 ·
				<span style="font-size:12px;color:rgba(255,255,255,0.6);margin-left:5px;font-weight:normal">（嘉宾排名顺序不分先后）</span>
			</div>
			<div class="judge">
				<img src="./img/person.png" alt="">
				<!-- <ul>
					<li class="judgeItem" v-for="(item,index) in people" :key="index">
						<div class="judgeImg">
							<div class="imgContain">
								<img :src="item.logo" alt="" />
							</div>
						</div>
						<div class="judgeName">
							{{item.name}}
						</div>
						<div class="judgeCompany">
							{{item.company}}
						</div>
						<div class="judgePosition">
							{{item.position}}
						</div>
					</li>
				</ul>
				<div class="judgetext">嘉宾评委团 持续邀约中...</div> -->
			</div>
			<!-- 启动仪式 -->
			<div class="headlineright" style="width:73.6%;margin-top:46px;">· 特邀嘉宾 ·</div>
			<div class="orgPeo">
				<img src="./img/org.png" alt="">
			</div>
			<div class="headlineleft" style="width:73.6%;margin-top:46px">· 系列路演日程 ·</div>
			<div class="series" style="clear:both">
				<div class="tableheader">
					<div>
						序号
					</div>
					<div>
						活动名称
					</div>
					<div>
						拟定举办时间
					</div>
				</div>
				<div class="tableBody" v-for="(item,index) in active" :key="index" :class="item.time.indexOf('已结束') > 0?'srecialColor':''">
					<div>
						{{index+1}}
					</div>
					<div>
						{{item.name}}
					</div>
					<div>
						{{item.time}}
					</div>
				</div>
			</div>
			<!-- 组委会介绍 -->
			<div class="headlineright" style="width:73.6%;margin-top:48px;">
				· 组委会介绍 ·
			</div>
			<div class="committee" style="clear:both">
				前海科控是深圳市前海管理局全资直属的三家平台公司之一，通过聚焦科创产业空间运营、高端科技专业服务、科创及文创产业投资等核心业务，努力打造前海科创产业投资运营服务平台，快速推动前海科技创新产业集聚发展。
				<br/><br/>
				第一路演是领先的人工智能路演平台，主要为新兴成长企业、VC/PE投后项目、产业园区项目、双创赛事项目提供融资路演服务，参与策划深圳金博会、高交会等大型活动，平台与主流投资机构紧密合作，基于大数据及人工智能算法对机构投资风格的精准画像，为路演企业精准匹配潜在投资者。
			</div>
			<div class="signup">
				<ul>
					<li>
						<router-link to="/roadshow">
							<span>路演项目</span>
							<span>报名 > </span>
						</router-link>
					</li>
					<li>
						<router-link to="/guest">
							<span>嘉宾评委</span>
							<span>报名 > </span>
						</router-link>
					</li>
					<li>
						<router-link to="/industry">
							<span>前海产业</span>
							<span>对接 > </span>
						</router-link>
					</li>
					<li>
						<router-link to="/media">
							<span>媒体/商务</span>
							<span>合作 > </span>
						</router-link>
					</li>
				</ul>
			</div>
			<!-- 路演报名表单 -->
			<div class="singupFormContain" style="margin-top:68px;">
				<div class="singupForm">
					<span class="signtitle">· 参会报名 ·</span>
					<div class="airborne">报名后携名片凭参会短信入场，谢绝空降。</div>
					<div class="radioSingle" @click="changeRadio()" style="display:none">
						<span>选择路演场次（多选）</span>
						<span> > </span>
					</div>
					<div class="projectItem">
						<span v-for="(item,index) in radiodata" :key="index">
							{{item.roadShowName}}
						</span>
					</div>
					<input type="text" placeholder="姓名" v-model="form.name">
					<input type="text" placeholder="公司名称" v-model="form.company">
					<input type="text" placeholder="职位" v-model="form.position">
					<input type="text" placeholder="微信" v-model="form.wechat">
					<input type="text" placeholder="手机" v-model="form.phone">
					<button @click="submit()">提交</button>
				</div>
			</div>
			<div class="tableContain">
				<!-- 剩余报名人数 -->
				<div class="residue">
					剩余报名名额：{{98 - tableList.length >= 0? 98 - tableList.length:0}}
				</div>
				<div class="interested">
                    <ul class="interestedUL">
                        <li class="interestedLi" v-for="(item,index) in tableList" :key="index">
                            <span>
                                {{tableList.length - index}}
                            </span>
                            <span>
                                {{item.name}}
                            </span>
                            <span>
                                {{item.companyName}}
                            </span>
                            <span>
                                {{item.position}}
                            </span>
                            <span>
                                {{item.phoneNo}}
                            </span>
                        </li>
                    </ul>
                </div>
			</div>
			<div class="imgcontain">
				<img src="./img/code.png" alt="">
			</div>
			<div class="adressContain">
				<div class="adress">
					<span>
						活动地址：<a href="http://apis.map.qq.com/uri/v1/marker?marker=coord:22.518,113.90;title:前海深港青年梦工场2号楼;addr: 广东省深圳市南山区前海深港合作区前海深港青年梦工场">前海深港青年梦工场2-104</a>
					</span>
					<span>
						公交路线：最近的地铁站是1号线鲤鱼门（出站后打车8分钟）、11号线南山站（车程15分钟）
					</span>
				</div>
			</div>
		</div>
		<!-- 单选 -->
		<!-- <singleradio v-if="radioSingle" v-model="radioSingle" @radioMethods="radioMethods"></singleradio> -->
		<checkradio v-if="radioSingle" v-model="radioSingle" @checkBoxclick="checkBoxclick"></checkradio>

		<div class="tosignup" @click="joinTable()" v-if="joinFlag">
			参会报名
		</div>
		<div class="fourTab">
			<ul>
				<li>
					<router-link to="/roadshow">
						<span>项目路演</span>
						<span>报名</span>
					</router-link>
				</li>
				<li>
					<router-link to="/guest">
						<span>嘉宾评委</span>
						<span>报名</span>
					</router-link>
				</li>
				<li>
					<router-link to="/industry">
						<span>前海产业</span>
						<span>对接</span>
					</router-link>
				</li>
				<li>
					<router-link to="/media">
						<span>媒体/商务</span>
						<span>合作</span>
					</router-link>
				</li>
			</ul>
		</div>
	</div>
</template>

<script>
import { Toast } from 'mint-ui';
import people from './people.js';
import active from './active.js';
import singleradio from './singleradio';
import checkradio from './checkradio';
export default {
	data () {
		return {
			people:people,
			active:active,
			radioSingle:false,
			radiodata:'',
			form:{
				name:'', // 名字
				company:'', // 公司
				position:'', // 职位
				wechat:'', // 微信
				phone:'', // 电话号码
			},
			tableList:[], // 报名列表数据
			domain:'https://app.dyly.com',
			joinFlag:false, // 参会报名显示和隐藏
			title:'【邀请函】“一带一路” 前海国际路演中心·巴西-葡萄牙科创企业专场路演',
			decs:'路演时间：9月11日14:00 路演地点：前海深港青年梦工场 智汇全球·追梦前海>>',
			imgUrl:'https://m.dyly.com/register/app_h5/img/qh.jpg',
			sharehref:'https://m.dyly.com/register/app_h5/qh/index.html'
		}
	},
	created(){
		// ModalHelper.afterOpen();
		this.listenBody(); // 页面滚动
		this.getTableList();
		this.share();
	},
	mounted(){
		var that = this;
		var audio = $('audio').get(0);
            //   audio.play();
		$('.icon-video').click(function () {
			if (audio.paused) {
				audio.play();
			} else {
				audio.pause();
			}
		})

		$(document).ready(function () {
			that.autoPlayMusic();
            that.audioAutoPlay();
		});
	},
	methods:{
		change(){ // 中英文切换
			let locale = this.$i18n.locale;
			locale === 'zh' ? this.$i18n.locale = 'en' : this.$i18n.locale = 'zh'
		},
		checkBoxclick(data){ // 多选按钮完成动作
			this.radiodata = data;
			this.radioSingle = false;
		},
		changeRadio(){ // 
			this.radioSingle = true;
		},
		submit(){ // 提交报名
		
			if(!this.form.name){
				Toast({
					message: '请填写姓名',
					iconClass: 'iconfont  icon-dingdanzhuangtaishibai'
				})
				return;
			}
			if(!this.form.company){
				Toast({
					message: '请填写公司',
					iconClass: 'iconfont  icon-dingdanzhuangtaishibai'
				})
				return;
			}
			if(!this.form.position){
				Toast({
					message: '请填写职位',
					iconClass: 'iconfont  icon-dingdanzhuangtaishibai'
				})
				return;
			}
			if(!this.form.wechat){
				Toast({
					message: '请填写微信',
					iconClass: 'iconfont  icon-dingdanzhuangtaishibai'
				})
				return;
			}
			if(!this.form.phone){
				Toast({
					message: '手机号为空或者手机号格式不正确',
					iconClass: 'iconfont  icon-dingdanzhuangtaishibai'
				})
				return;
			}

			this.axios.post(this.domain+'/vc/qhRoadShow/signUp',{
				"companyName": this.form.company, // 公司名
				"name": this.form.name, //姓名
				"position": this.form.position, // 职位
				"phoneNo": this.form.phone, // 手机号
				"wxNum": this.form.wechat, // 微信
			 	"roadshowId":"2",
				"type": "3",
				"language": "0"
			}).then((res)=>{
				if(res.data.status == 1){
					Toast({
						message: '报名成功',
						iconClass: 'iconfont  icon-chenggong'
					})
					this.getTableList();
				}else{
					Toast({
						message: '报名失败',
						iconClass: 'iconfont  icon-dingdanzhuangtaishibai'
					})
				}
			})
		},
		listenBody(){ // 滚动监听
			var that = this;
			$(window).scroll(function() {
				var scrollTop = document.documentElement.scrollTop || window.pageYOffset || document.body.scrollTop;
				var h = $(document).height();
				if(scrollTop  > window.screen.height /4){ // 一个整屏幕高度
					that.joinFlag = true;
					// if(h - scrollTop < 1400){
					// 	that.joinFlag = false;
					// }
				}else{
					that.joinFlag = false;
				}
			})
		},
		joinTable(){ // 参与报名
			var top = $('.singupFormContain').offset().top; // 报名参与的高度
			$('body,html').animate({
				scrollTop: top - 100
			}, 400);
		},
		share(){
			var that = this;
			$.getScript('https://res.wx.qq.com/open/js/jweixin-1.0.0.js', function(){
				$.ajax({
					url: "https://m.dyly.com/weixin/getWxConfig",
					type: 'POST',
					data: {
						url: window.location.href
					}
				}).success(function(data){
					wx.config({
						appId: data.data.appId,
						timestamp: data.data.timestamp,
						nonceStr: data.data.nonceStr,
						signature: data.data.signature,
						jsApiList: ['onMenuShareTimeline','onMenuShareAppMessage']
					});
					// updateAppMessageShareData
					wx.ready(function(){
						// 朋友圈分享
						wx.onMenuShareTimeline({
							title: that.title,
							link: window.location.href,
							imgUrl: that.imgUrl
						})
						// 分享给朋友
						wx.onMenuShareAppMessage({
							title: that.title,
							desc: that.decs,
							link: window.location.href,
							imgUrl: that.imgUrl
						})
					})
				})
			});
		},

		// 音乐播放
		autoPlayMusic() {
			var that = this;
                // 自动播放音乐效果，解决浏览器或者APP自动播放问题
			function musicInBrowserHandler() {
				that.musicPlay(true);
				document.body.removeEventListener('touchstart', musicInBrowserHandler);
			}
			document.body.addEventListener('touchstart', musicInBrowserHandler);
			// 自动播放音乐效果，解决微信自动播放问题
			function musicInWeixinHandler() {
				that.musicPlay(true);
				document.addEventListener("WeixinJSBridgeReady", function () {
					that.musicPlay(true);
				}, false);
				document.removeEventListener('DOMContentLoaded', musicInWeixinHandler);
			}
			document.addEventListener('DOMContentLoaded', musicInWeixinHandler);
		},
		musicPlay(isPlay) {
			var media = document.querySelector('#bg-music');
			if (isPlay && media.paused) {
				media.play();
			}
			if (!isPlay && !media.paused) {
				media.pause();
			}
		},
		audioAutoPlay() {
			var audio = document.getElementById('bg-music');
			audio.play();
			document.addEventListener("WeixinJSBridgeReady", function () {
				audio.play();
			}, false);
		},
		getTableList(){ // 获取报名列表
			this.axios.get(this.domain +'/vc/qhRoadShow/getSignUpList',{
				params:{
					"roadShowId":2
				}
			}).then((res)=>{
				if(res.data.status == 1){
					this.tableList = res.data.data?res.data.data:[];
				}
			})
		}
	},

	components:{
		"singleradio":singleradio,
		"checkradio":checkradio,
		"Toast":Toast
	},
	destroyed(){
        // ModalHelper.beforeClose();
    }
	
}
</script>
<style lang="scss">
	.homePage{
		width:100%;
		height:auto;
		background-color:#01040D;
		padding-top: 40px;
		.homebg{
			width:100%;
			position:relative;
			.homeTitlebg{
				display:block;
				width:100%;
				height:auto;
			}
			.homeText{
				width:100%;
				height:auto;
				display:block;
				position:absolute;
				top:80px;
				z-index:1;
			}
			.unit{
				width:100%;
				position:absolute;
				left:0;
				bottom:164px;
				z-index:1;
				padding-left:26px;
				box-sizing: border-box;
				span{
					display:block;
					color:rgba(98,178,232,0.8);
					font-size:13px;
					line-height:22px;
				}
			}
			.icon-video{
				width: 30px;
				height: 30px;
				position: fixed;
				right: 15px;
				top: 44px;
				background: url('https://static.dyly.com/yuegangao/video.svg');
				z-index: 2;
				background-size: 100%;
			}
			.transform{
				animation: transform 3.5s linear infinite;
			}
		}
		.homeBody{
			width:100%;
			background:url('./img/bg2.png') repeat-y;
			background-size:100%;
			background-color:#01040D;
			position:relative;
			z-index:1;
			margin-top:-85px;
			padding-bottom:30px;
			.timeShaft{
				width:100%;
				padding:37px 19px 50px 19px;
				box-sizing: border-box;
				.timeShiftimg{
					width:100%;
					height:auto;
				}
				ul{
					width:100%;
					li{
						position:relative;
						display:flex;
						width:100%;
						height:44px;
						box-sizing: border-box;
						span:nth-child(1){
							width:16px;
							height:16px;
							border:1px dashed rgba(65,179,243,1);
							border-radius: 50%;
							display:flex;
							align-items: center;
							justify-content: center;
							i{
								width:8px;
								height:8px;
								display:inline-block;
								border-radius: 50%;
								background:rgba(65,179,243,1);
							}
						}
						span:nth-child(2){
							width:77px;
							color:rgba(65,179,243,1);
							font-size:14px;
							margin-left:16px;
							display:inline-block;
							margin-top:2px;
						}
						span:nth-child(3){
							color:rgba(217,240,249,1);
							font-size:14px;
							margin-left:16px;
							display:inline-block;
						}
						&:after{
							content:'';
							display:block;
							position:absolute;
							border-left:1px dashed rgba(65,179,243,1);
							width:2px;
							height:22px;
							top: 21px;
    						left: 8px;
						}
						&:last-child{
							&:after{
								height:0px;
							}
						}
					}
				}
			}
			.projectItemList{
				width:100%;
				padding: 0 16px;
				box-sizing: border-box;
				img{
					width:100%;
					height:auto;
				}
			}
			.roadProject{
				width:100%;
				padding:6px 16px 0 16px;
				box-sizing: border-box;
				clear: both;
				ul{
					width:100%;
					background:rgba(59,150,210,0.15);
					box-sizing: border-box;
					padding:24px 10px 20px 25px;
					li{
						font-size:13px;
						color:rgba(98,178,232,1);
						line-height:22px;
						list-style: disc;
						&:nth-child(1){
							font-size:15px;
							font-weight: bold;
							color:rgba(217,240,249,1);
							line-height:24px;
							margin-bottom:5px;
							list-style:none;
						}
					} 
				}
			}
			.judge{
				width:100%;
				height:auto;
				padding:24px 16px 0px 16px;
				box-sizing: border-box;
				ul{
					width:100%;
					display:flex;
					flex-warp:warp; /*CSS3样式，支持webkit，ms*/
					-ms-flex-wrap: wrap;/*IE9以及一下不支持*/
					-webkit-flex-wrap: wrap;
					li{
						width:25%;
						display:flex;
						flex-direction: column;
						align-items: center;
						margin-bottom:20px;
						.judgeImg{
							width:70px;
							height:70px;
							border:1px dashed rgba(65,179,243,1);
							border-radius: 50%;
							display: flex;
							align-items: center;
							justify-content: center;
							.imgContain{
								width:60px;
								height:60px;
								border-radius: 50%;
								background:rgba(65,179,243,1);
								display:flex;
								align-items: center;
								justify-content: center;
								img{
									width:100%;
									height:auto;
									display:block;
									border-radius: 50%;
								}
							}
						}
						.judgeName{
							font-size: 14px;
							font-weight:bold;
							color:rgba(65,179,243,1);
							margin-top:10px;
						}
						.judgeCompany{
							font-size:12px;
							color:rgba(255,255,255,0.6);
							margin-top:2px;
						}
						.judgePosition{
							font-size:12px;
							color:rgba(255,255,255,0.6);
							margin-top:2px;
						}
					}
				}
				.judgetext{
					width:100%;
					text-align: center;
					font-size:14px;
					color:rgba(98,178,232,1);
					margin-top:10px;
				}
				img{
					display:block;
					width:100%;
					height:auto;
				}
			}
			.series{
				width:100%;
				padding:25px 16px 0 16px;
				box-sizing: border-box;
				color:rgba(132,189,255,1);
				line-height:16px;
				.tableheader{
					height:30px;
					width:100%;
					display:flex;
					margin-bottom:1px;
					div{
						height:100%;
						background:rgba(59,150,210,0.15);
						font-size:12px;
						display:flex;
						align-items: center;
						&:nth-child(1){
							width:44px;
							margin-right: 1px;
							justify-content: center;
						}
						&:nth-child(2){
							padding-left:10px;
							box-sizing: border-box;
							width:calc(100% - 140px);
							margin-right: 1px;
						}
						&:nth-child(3){
							width:92px;
							justify-content: center;
						}
					}
				}
				.tableBody{
					height:52px;
					width:100%;
					display:flex;
					margin-bottom:1px;
					div{
						height:100%;
						background:rgba(59,150,210,0.15);
						font-size:12px;
						display:flex;
						align-items: center;
						&:nth-child(1){
							width:44px;
							margin-right: 1px;
							justify-content: center;
						}
						&:nth-child(2){
							padding-left:10px;
							box-sizing: border-box;
							width:calc(100% - 140px);
							margin-right: 1px;
						}
						&:nth-child(3){
							width:92px;
							justify-content: center;
							text-align: center;
						}
					}
				}
				.srecialColor{
					color:rgba(255,255,255,0.3);
				}

			}
			.committee{
				width:100%;
				padding:32px 24px 0 24px;
				box-sizing: border-box;
				color:rgba(98,178,232,0.8);
				line-height:22px;
				font-size:14px;
			}
			.signup{
				width:100%;
				margin-top:50px;
				padding:0 24px;
				box-sizing: border-box;
				ul{
					width:100%;
					display:flex;
					align-items: center;
					justify-content: space-between;
					height:80px;
					li{
						width:70px;
						height:100%;
						background:url('./img/db.png');
						background-size: cover;
						a{
							width:100%;
							height:100%;
							display:flex;
							flex-direction: column;
							align-items: center;
							justify-content: center;
							font-size:13px;
							color:rgba(255,255,255,1);
							line-height:18px;
							text-decoration: none;
						}
					}
				}
			}
			.imgcontain{
				width:100%;
				padding:0 16px 0px 16px;
				margin-top:20px;
				box-sizing: border-box;
				img{
					width:100%;
					height:auto;
				}
			}
			.tableContain{
				width:100%;
				padding: 0 16px;
				box-sizing: border-box;
				margin-top:48px;
				.residue{
					width:100%;
					font-size:14px;
					color:#ffffff;
					display:flex;
					justify-content: center;
					margin-bottom: 20px;
				}
				.interestedUL{
					width:100%;
				}
				.interestedLi{
					width: 100%;
					height: 35px;
					display:flex;
					background:rgba(59,150,210,0.15);
					border-radius:2px;
					margin-bottom: 1px;
				} 
				.interestedLi:last-child{
					margin-bottom: none;
				}
				.interestedLi span{
					height: 100%;
					line-height: 35px;
					text-align: center;
					font-size:0px;
					color:rgba(255,255,255,0.6);
					overflow: hidden;/*超出部分隐藏*/
					white-space: nowrap;/*不换行*/
					text-overflow:ellipsis;/*超出部分文字以...显示*/
				}
				.interestedLi span:nth-child(1){
					width:10%;
					font-size:12px;
				}
				.interestedLi span:nth-child(2){
					width:20%;
					font-size:12px;
				}
				.interestedLi span:nth-child(3){
					width:20%;
					font-size:12px;
				}
				.interestedLi span:nth-child(4){
					width:20%;
					font-size:12px;
				}
				.interestedLi span:nth-child(5){
					width:30%;
					font-size:12px;
				}
			}
			.orgPeo{
				width:100%;
				padding:32px 16px 0 16px;
				height:auto;
				clear:both;
				box-sizing: border-box;
				img{
					display:block;
					width:100%;
					height:auto;
				}
			}
			.adressContain{
				width:100%;
				padding:20px 16px;
				box-sizing: border-box;
				.adress{
					width:100%;
					padding:20px;
					box-sizing: border-box;
					background:rgba(59,150,210,0.15);
					border-radius:4px;
					font-size:14px;
					color:rgba(217,240,249,1);
					line-height:20px;
					display:flex;
					flex-direction: column;
					span{
						&:nth-child(1){
							margin-bottom:5px;
						}
					}
					a{
						color:#41B3F3;
						text-decoration: none;
					}
				}
			}
			
		}
		.tosignup{
			width:100%;
			height:40px;
			background:rgba(1,79,125,0.95);
			color:#ffffff;
			font-size:14px;
			position:fixed;
			bottom:0;
			z-index: 10;
			display:flex;
			align-items: center;
			justify-content: center;
			max-width: 750px;
		}
		.fourTab{
			width:100%;
			max-width: 750px;
			height:40px;
			background:rgba(1,79,125,0.95);
			color:#ffffff;
			position:fixed;
			top:0;
			z-index:2;
			ul{
				width:100%;
				display:flex;
				li{
					width:25%;
					height:100%;
					border-right:1px solid rgba(2,8,22,0.15);
					a{
						width:100%;
						height:100%;
						color:#ffffff;
						display:flex;
						flex-direction:column;
						font-size: 12px;
						align-items: center;
						justify-content: center;
						text-decoration: none;
						span{
							&:nth-child(1){
								margin-top:2px;
							}
						}
					}
				}
			}
		}
	}
	@-webkit-keyframes transform {
		0% {
			-webkit-transform: rotateZ(0);
			transform: rotateZ(0)
		}

		100% {
			-webkit-transform: rotateZ(360deg);
			transform: rotateZ(360deg)
		}
	}

	@keyframes transform {
		0% {
			-webkit-transform: rotateZ(0);
			transform: rotateZ(0)
		}

		100% {
			-webkit-transform: rotateZ(360deg);
			transform: rotateZ(360deg)
		}
	}

	#bg-music {
		width: 0;
		height: 0;
		overflow: hidden;
		display: block;
		right: 0;
	}
	.airborne{
		display:flex;
		justify-content: center;
		font-size:12px;
		color:rgba(65,179,243,1);
		margin-bottom:16px;
	}
</style>
