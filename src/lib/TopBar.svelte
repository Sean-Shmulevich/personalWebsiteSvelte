<script>
    import '../css/98.css';
    import '../css/myStyle.css';

    import linkedIn from '../assets/linkedin_pixel_logo_icon_181925.png';
    import instaLogo from '../assets/instagram_pixel_logo_icon_181922.png';
    

    var today = new Date();
    //first 3 letters of the current month
    let monthStr = (new Intl.DateTimeFormat('en-US', { month: "long" }).format(today)).substring(0,3);
    let dayOfWeek = (new Intl.DateTimeFormat('en-US', { weekday: 'long' }).format(today)).substring(0,3);
    let dayOfMonth = (new Intl.DateTimeFormat('en-US', { day: 'numeric' }).format(today));
</script>
<div class="notAButton notMyToolBar topBar">
    <div class="nameBorder">
        <h1 class="street">Sean Shmulevich</h1>
        <!--<img src="./favicon.svg" class="leftIcon" alt="hello alt">-->
    </div>
    <div class="rightBox">
        <!--<img src="https://win98icons.alexmeub.com/icons/png/magnifying_glass-0.png" alt="hello alt" class="rightmost" style="margin-right: 4mm;">-->
        <span class="dateText">{dayOfWeek} {monthStr} {dayOfMonth}</span>
        <a href="https://github.com/Sean-Shmulevich"  target="_blank" rel="noopener noreferrer"><img src="https://pixelartmaker-data-78746291193.nyc3.digitaloceanspaces.com/image/d7e4e1e509c728d.png" alt="Sean shmulevich github link" class="rightmost" style="margin-left:-3px"></a>
        <a href="https://www.linkedin.com/in/sean-shmulevich-237190185/" target="_blank" rel="noopener noreferrer"><img src={linkedIn} alt="Sean Shmulevich LinkedIn link" class="rightmost"></a>
        <a href="https://www.instagram.com/theshmulconspiracy/" target="_blank" rel="noopener noreferrer"><img src={instaLogo} alt="Sean Shmulevich instagram link" class="rightmost"></a>
    </div>
</div>
<style>
    /* .leftIcon {
        width: 54px;
        max-height: 45px;
        margin-top: -10px;
        vertical-align: middle;
    } */
    a:focus{
        outline: unset;
    }
    .nameBorder{

        width: 300px;
        min-width: 150px;
        overflow: hidden;
        height: 30px;
        max-height:30px;
        display: flex; 
        margin-top: 0px;


        background: rgb(174, 168, 217);
    }
  .street {
        white-space: nowrap;
        position: relative;
        font-family: 'Apple Garamond bold', sans-serif;
        font-size: 38px;
        font-style: italic;
        -webkit-text-stroke: 2px rgba(0, 0, 0, 0.35);
        color: rgb(40,40,77);
        background: -webkit-linear-gradient(60deg, rgb(154 143 233), rgb(26 26 101) );
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        margin: 0;
        margin-right: auto;
        margin-top: -6px;
        margin-left: 0px;
      }
    .dateText{
        white-space: nowrap;
        color: black;
        font-family: 'Apple Garamond bold';
        font-size: 1.5rem;
        margin-right: 20px;
        margin-left: -3px;
    }
    .rightBox{
        display: inline-flex;
        flex-direction: row-reverse;
    }
    .topBar {
        align-items: center;
        height: 36px;
        position: fixed;
    }
    .rightmost {
        /*transform: scaleX(-1);*/
        width:22px;
        max-height: 23px;
        vertical-align: middle;
        margin-left:auto;
        margin-right: 20px;
        margin-top: 2px;
    }
</style>