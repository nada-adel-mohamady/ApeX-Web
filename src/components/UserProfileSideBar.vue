<template id="profilesidebardesign">
<div id='sidebar'>
<div id="main">
    <div class="box" id="infobox">
        <div class="bluebackgroung">
          <div class="img">
             <img width="100%" class="image" :src="'http://35.232.3.8'+image" />
          </div>
        </div>
        <div class="content">
          <h4 class="username" v-show="fullName==null"> {{userName}} </h4>
          <h4 class="username" > {{fullName}} </h4>
<div class="info">
  <div style="display:inline; float:left; width:50%;">
    <h5 class="font"  id="karmacount">karma</h5>
    <svg style="display:inline;" class="svg" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 viewBox="0 0 20 20"  xml:space="preserve">

<path class="karma" d="M7.509604,9.809682c0.092814-1.228464,1.071614-2.207275,2.30009-2.300069
	C8.787232,6.158976,7.167115,5.28595,5.34253,5.28595h-0.0566v0.05657C5.28593,7.167094,6.158977,8.787262,7.509604,9.809682z"/>
<path class="karma" d="M7.509604,10.190318c-1.350626,1.02242-2.223673,2.642588-2.223673,4.467163v0.056569h0.0566
	c1.824585,0,3.444703-0.873027,4.467164-2.223663C8.581218,12.397593,7.602417,11.418773,7.509604,10.190318z"/>
<path class="karma" d="M12.490397,10.190318c-0.092813,1.228455-1.071614,2.207275-2.300089,2.300069
	c1.022461,1.350636,2.642578,2.223663,4.467163,2.223663h0.0566v-0.056569
	C14.714071,12.832906,13.841024,11.212738,12.490397,10.190318z"/>
<path class="karma" d="M14.657472,5.28595c-1.824585,0-3.444702,0.873026-4.467163,2.223663
	c1.228475,0.092794,2.207275,1.071605,2.300089,2.300069c1.350627-1.02242,2.223674-2.642588,2.223674-4.467163V5.28595H14.657472z"
	/>
<path class="karma" d="M16.626669,9.960002c-0.674195-0.674205-1.478618-1.135641-2.331503-1.393779
	C13.962443,9.098622,13.546,9.582967,13.051677,10c0.494324,0.417043,0.910767,0.901378,1.243489,1.433777
	c0.852885-0.258138,1.657308-0.719574,2.331503-1.393779L16.666666,10L16.626669,9.960002z"/>
<path class="karma" d="M10,6.948313c0.417033-0.494324,0.901387-0.910756,1.433797-1.243479
	c-0.258138-0.852885-0.719604-1.657288-1.393799-2.331502L10,3.333333L9.960002,3.373332
	C9.285808,4.047536,8.824341,4.851949,8.566203,5.704834C9.098613,6.037557,9.582967,6.45399,10,6.948313z"/>
<path class="karma" d="M6.948324,10C6.454,9.582967,6.037557,9.098622,5.704834,8.566223C4.851949,8.824361,4.047526,9.285797,3.373332,9.960002
	L3.333333,10l0.039999,0.039998c0.674194,0.674205,1.478617,1.135641,2.331502,1.393779
	C6.037557,10.901378,6.454,10.417043,6.948324,10z"/>
<path class="karma" d="M10,13.051686c-0.417033,0.494324-0.901387,0.910757-1.433797,1.24348
	c0.258138,0.852885,0.719604,1.657298,1.393799,2.331503L10,16.666666l0.039998-0.039997
	c0.674194-0.674215,1.135661-1.478618,1.393799-2.331503C10.901387,13.962443,10.417033,13.54601,10,13.051686z"/>
</svg>
<h5 style="display:inline; color:#7c7c7c;" id="karmanumber" > {{karmaCount}} </h5>

  </div>
  <div style="display:inline; float:right; width:50%;">
    <h5 class="font"  id="cakeday">cake day</h5>

<svg style="display:inline;" class="svg2" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 width="512px" height="512px" viewBox="0 0 512 512" enable-background="new 0 0 512 512" xml:space="preserve">
<g>
	<path class="karma" d="M454.928,237.161l-32.273-89.114c-5.769-15.921-22.479-25.068-38.994-21.332l-51.145,11.539
		c5.249,9.184,8.488,19.664,8.488,30.978c0,34.705-28.228,62.926-62.924,62.926c-34.686,0-62.908-28.221-62.908-62.926
		c0-1.577,0.35-3.056,0.464-4.604L73.409,196.723c-15.695,3.542-26.84,17.482-26.84,33.582v192.493
		c0,24.713,18.545,45.151,43.136,47.555l314.833,30.707c1.535,0.146,3.071,0.228,4.605,0.228c11.894,0,23.298-4.402,32.104-12.379
		c9.969-9.034,15.687-21.934,15.687-35.403V248.599C456.934,244.7,456.252,240.817,454.928,237.161z M82.362,242.247
		c1.599-1.462,3.744-2.161,5.905-1.95l328.465,32.022c3.931,0.391,6.929,3.688,6.929,7.653v77.395
		c-1.594,0.597-3.189,1.232-4.59,2.346c-3.785,3.021-8.708,4.45-13.549,3.866c-4.988-0.617-9.432-3.103-12.528-7.002l-1.136-1.381
		c-8.75-10.383-21.373-17.206-34.899-18.798c-13.525-1.641-26.75,1.835-37.684,9.651l-2.169,1.624
		c-3.858,3.071-8.676,4.5-13.614,3.834c-4.647-0.552-8.806-2.73-11.821-6.157l-0.657-0.829
		c-18.449-23.348-52.503-27.344-75.866-8.92l-0.797,0.634c-3.777,2.666-8.351,3.835-13.03,3.234
		c-4.791-0.538-9.269-3.04-12.306-6.906c-8.944-11.339-21.747-18.505-36.083-20.21c-14.168-1.657-28.644,2.452-39.822,11.258
		c-3.908,3.088-8.798,4.404-13.672,3.883c-4.915-0.567-9.31-3.038-12.388-6.938c-1.931-2.445-4.491-3.929-7.205-4.962v-67.661
		C79.843,245.755,80.761,243.692,82.362,242.247z M418.909,464.246c-2.682,2.436-6.15,3.768-9.766,3.768L92.938,437.242
		c-7.465-0.73-13.095-6.938-13.095-14.444v-66.975c17.17,7.94,38.045,6.402,53.94-6.103c4.256-3.381,9.854-4.956,15.248-4.322
		c5.499,0.65,10.421,3.412,13.842,7.75c8.49,10.804,21.145,17.871,34.565,19.367c13.771,1.706,27.336-2.112,38.277-10.722
		l0.919-0.715c8.668-6.143,20.691-4.712,27.669,3.347l0.601,0.764c8.555,10.835,20.853,17.725,34.663,19.365
		c12.917,1.496,25.629-1.738,36.1-9.228l2.138-1.576c4.337-3.429,9.764-4.922,15.248-4.305c5.41,0.634,10.421,3.429,13.761,7.685
		l1.219,1.462c8.489,10.025,20.309,16.394,33.525,18.018c1.99,0.228,3.979,0.341,5.971,0.341c5.497,0,10.939-0.946,16.133-2.635
		v59.19C423.66,457.599,421.931,461.516,418.909,464.246z"/>
	<path class="karma" d="M215.497,36.334c48.088,27.136,53.64,87.477,53.645,87.517c-21.248,4.181-37.333,22.92-37.333,45.382
		c0,25.524,20.754,46.289,46.271,46.289c25.524,0,46.287-20.764,46.287-46.289c0-23.25-17.285-42.362-39.648-45.615
		c0.008-0.422,4.48-74.546-53.234-116.464c-8.058-4.419-18.179-1.461-22.583,6.596C204.481,21.808,207.372,31.749,215.497,36.334z"
		/>
</g>
</svg>
<!-- <h5 style="display:inline; font-size: 14px; color:#7c7c7c;" id="cakedaynumber" > {{cakeDay}} </h5> -->
  </div>
</div>
          <button v-show="notGuest&&!settings" id="createpostbutton" class="button" type="button" v-on:click="createPost()">new post</button>
          <button v-show="!notGuest&&!settings" v-on:click="blockUser()" id="blocktbutton" class="button" type="button">block</button>
          <button v-show="isAdmin&&!settings&&!notGuest" v-on:click="deleteUser()" id="deletebutton" class="button" type="button">delete user</button>
        </div>
    </div>
    </div>
</div>
</template>

<script>
import {AllServices} from '../MimicServices/AllServices.js'
import swal from 'sweetalert'

/**
 * @vue-data {JWT} [token='']  user Token
 * @vue-data  {string} image - Url of user profile image
 * @vue-data  {number} KarmaCount - Number of karma
 * @vue-prop {string} UserName - Name of user
 * @vue-prop {string} settings - indicates wether the comonent is called in profile or settings
 * @vue-data  {boolean} [isAdmin=false] - boolean indicates if the user is moderator or not
 * @vue-data  {boolean} [notGuest=false] - boolean indicates if the user is in his profile or other user profile
 * @vue-data {string} id - user id
 * @vue-data {string} cakeDay - date when this profile was created
 * @vue-data {string} fullName - user full name
 * @vue-data {string} loggeduser  name of logged in user
 * @vue-data {boolean} loggedIn  check if user is logged in
 */

export default {
  props:{
      userName:String,
      settings:Boolean,
       },
  data () {
    return {
      token:this.$localStorage.get('token'),
      loggedIn:this.$localStorage.get('login'),
      loggeduser:this.$localStorage.get('userName'),
      karmaCount:0,
      image:'',
      // cakeDay:'',
      fullName:'',
      id:'',
      isAdmin:false,
      notGuest:false,
    }
  },
  methods:
  {
  /**
    * check if the user if Admin
    */
    isAdminFunction:function(){
      AllServices.userType().then((data) =>{
        if(data.user.type ==3){
          this.isAdmin= true;
          }
        else{
          this.isAdmin= false;
        }
      })
    },
    /**
    * used to block user
    */
    blockUser:function(){
    if(this.loggedIn){
     AllServices.blockUser(this.id).then((data) =>{
     if(data){
         swal('this user have been blocked successfully');
         this.$router.push({name:'HomePage'});
       }
       else{
         swal('sorry something worng happend');
       }
       })
       }
      else{
        swal('you have to log in first');
      }
    },
    /**
    * check if the user requesting his profile or other user profile
    */
    notGuestFunction:function(){
      if(this.userName != this.loggeduser){
        this.notGuest= false;
      }
      else{
        this.notGuest= true;
      }
    },
    /**
    * send request to delete user
    */
    deleteUser:function(){
      var response = AllServices.deleteUser(this.id);
      if(response){
      swal('Done :)');
      this.$router.push({name:'HomePage'});
    }
    else{
      swal('sorry something went wrong :)')
    }
    },
    /**
       * if user is logged in , can go to create post or create community
      */
      createPost: function(){
        if( this.loggedIn )
        {
          this.$router.push('/Submit');
        }
        else{
           this.$modal.show('demo-login');
        }
      },
    /**
    * get user profile info
    */
    getUserProfile:function(){ 
      AllServices.getUserInfo().then((data) =>{
      this.karmaCount = data.user_info[0].karma;
      this.image = data.user_info[0].avatar;
      this.id = data.user_info[0].id;
      this.fullName = data.user_info[0].fullname;
      })
   },
    /**
    * get user account data for another user
    */
   getUserData:function(){
      AllServices.getUserInfoById(this.userName).then((data) =>{
      this.karmaCount = data.userData.karma;
      this.image = data.userData.avatar;
      this.id = data.userData.id;
      this.fullName = data.userData.fullname;
      // this.cakeDay = data.userData.cakeDay;
      })
   },
   /**
    * get user account data for a guset
    */
   getUserDataForGuest:function(){
     AllServices.getUserInfoByIdforGuest(this.userName).then((data) =>{
      this.karmaCount = data.userData.karma;
      this.image =data.userData.avatar;
      this.id = data.userData.id;
      this.fullName = data.userData.fullname;
     })
   },
  },
  mounted(){
    if(this.loggedIn){
    if(this.userName == this.loggeduser){
      this.getUserProfile();

    }
    else{
      this.getUserData();
    }
    this.notGuestFunction();
    this.isAdminFunction();
    }
    else{
      this.getUserDataForGuest();
    }
  }
}
</script>

<style scoped>
*{
  box-sizing: border-box;
}
#sidebar{
  width:22%;
  float:right;
  margin-right:5%;
  margin-left:3%;
  margin-top: 5%;
}
.bluebackgroung{
  background-color: deepskyblue;
  padding-top: 12%;
  padding-bottom:0%;
  padding-left:4%;
  padding-right:65%;
  height: auto;
  border-top-left-radius: 20%;
  border-top-right-radius: 20%;
}
.image{
  border-radius: 10%;
}
.img{
  padding:2%;
  background-color: white;
  box-sizing: border-box;
  border-radius: 4px;
  margin-bottom:-15%;
  width:80px;
}
.content{
  background-color: white;
  height: auto;
  padding-top: 5%;
  padding-bottom:5%;
  padding-left:8%;
  padding-right:8%;
  border-bottom-left-radius: 20%;
  border-bottom-right-radius: 20%;
}
.name{
  font-size: 16px;
  font-weight: 500;
  color: rgb(34, 34, 34);
  margin-top: 4%;
}
.username{
  color: #7c7c7c;
  font-size: 16px;
}
.box{
  margin-bottom: 5%;
}
.button{
  width:100%;
  margin:2% 0%;
  background-color:skyBlue;
  color:white;
  padding: 1%;
  border-width: 3px;
  border-radius: 20%;
  cursor:pointer;
  border-color: skyblue;
  border-style: solid;
  font-size: 14px;
  font-weight: 500;
  letter-spacing: 0.5px;
  text-transform: uppercase;
  height:auto;
  overflow: hidden;
}
.button:hover {opacity: 0.75}

#karmanumber{
  font-size: 14px;
  font-weight: 400;
}
.Header{
  background-color: skyBlue;
  padding:4%;
  margin-top: 10%;
  margin-bottom: 0%;
  height:auto;
  border-top-left-radius: 20%;
  border-top-right-radius: 20%;
  font-size: 20px;
}
.karma{
  fill: skyBlue;
}
.svg{
  width:18%;
  height:auto;
  margin-top:0%;
  margin-left:0%;
  margin-right:0%;
  margin-bottom:-7%;
  padding-left:0%;
  padding-right:0%;
  padding-top:2%;
  padding-bottom:2%;
}
.svg2{
  width:14%;
  height:auto;
  margin-top:0%;
  margin-left:0%;
  margin-right:0%;
  margin-bottom:-3%;
  padding-left:0%;
  padding-right:0%;
  padding-top:2%;
  padding-bottom:1%;
}
.info{
  margin-top: 3%;
  margin-bottom: 3%;
  display: inline-block;
  width: 100%;
}
.font{
  font-size: 16px;
  font-weight: 500;
  color:#222;
}
.images{
  margin-top: 3%;
  margin-bottom: 3%;
}
.Header{
  background-color: skyBlue;
  padding:4%;
  margin: 0%;
  height:auto;
  border-top-left-radius: 20%;
  border-top-right-radius: 20%;
}
.contentblocklist{
  background-color: #eee;
  height: auto;
  padding-top: 5%;
  padding-bottom:5%;
  padding-left:8%;
  padding-right:8%;
  border-bottom-left-radius: 20%;
  border-bottom-right-radius: 20%;
}
#blocklistitam{
  width:100%;
  height: auto;
  display:inline-block;
  padding: 0%;
  margin:3%;
}
@media(max-width:960px){
  #sidebar{
    display:none
  }
}
</style>
