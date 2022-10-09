<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>same as new</title>
    <link rel="stylesheet" href="test.css">
  <style>
  * {
    box-sizing: border-box;
  }
  body {
    margin: 0;
  }
  .crm-container{
    display:flex;
    flex-direction:column;
    justify-content:center;
    position:relative;
    flex:1;
    margin-left:auto;
    margin-right:auto;
    max-width:calc(1 * var(--crm-section-container-max-width, 100%));
    width:100%;
    min-height:90px;
    padding:0px 10px;
  }
  .crm-section{
    display:block;
    position:relative;
  }
  .crm-section-inner{
    position:relative;
    display:flex;
    flex-direction:column;
    align-items:center;
  }
  .crm-section-padding{
    width:100%;
    height:100px;
    position:relative;
    cursor:default;
  }
  :root{
    --crm-section-container-max-width:1170px;
  }
  .crm-section-inner > .crm-shapeDivider-wrapper > .crm-shapeDivider{
    height:100px;
  }
  .crm-bg{
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    z-index:-1;
  }
  .crm-bg-color{
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
  }
  .crm-bg-image{
    position:absolute;
    top:0;
    left:0;
    width:100%;
    height:100%;
    background-repeat:no-repeat;
    background-size:cover;
  }
  .menu1-nav hr{
    width:90%;
    margin:auto;
    border-top:2px solid #d5d5d5;
    border-right:none;
    border-left:none;
    border-bottom:none;
  }
  .menu1-nav li:last-of-type > hr{
    display:none;
  }
  .menu1-nav ul{
    padding:0;
    margin:0;
    list-style:none;
    position:relative;
  }
  .menu1-nav ul li{
    display:inline-block;
  }
  .menu1-nav a{
    padding:0 10px;
    text-decoration:none;
    height:50px;
    display:flex;
    align-items:center;
    white-space:nowrap;
  }
  .menu1-nav a p{
    margin:0;
  }
  .menu1-nav ul li a{
    padding:10px 10px 10px 10px;
  }
  .menu1-nav ul li:hover{
    background-color:rgba(14, 164, 233, 1) !important;
  }
  .menu1-nav ul li:hover > ul{
    display:inherit;
  }
  .menu1-nav ul ul{
    display:none;
    position:absolute;
    top:106%;
  }
  .menu1-nav ul ul li{
    min-width:170px;
    float:none;
    display:list-item;
    position:relative;
    background-color:#fff;
  }
  .menu1-nav ul ul li a{
    padding:10px 10px 10px 10px;
  }
  .menu1-nav ul ul li:hover{
    box-shadow:none;
    background-color:#fff;
  }
  .menu1-nav ul ul ul{
    top:0%;
  }
  .menu1-nav ul ul ul li{
    position:relative;
    left:100%;
  }
  .menu1-nav li a i{
    padding-left:3px;
  }
  .menu1-nav li a i.up{
    display:none;
  }
  .menu1-nav ul li:hover > a i.up{
    display:inline;
  }
  .menu1-nav ul li:hover > a i.down{
    display:none;
  }
  .menu1-nav.menu-vertical{
    height:auto !important;
  }
  .menu1-nav.menu-vertical a{
    justify-content:center;
  }
  .menu1-nav.menu-vertical li{
    text-align:center;
    width:100%;
  }
  .menu1-nav.menu-vertical ul li{
    display:list-item;
  }
  .menu1-nav.menu-vertical ul li:hover > ul li{
    background-color:#e9e9e9;
  }
  .menu1-nav.menu-vertical ul ul{
    position:relative;
    top:0px;
  }
  .menu1-nav.menu-vertical ul ul ul li{
    position:relative;
    top:0px;
    left:0px;
  }
  i{
    text-align:center;
    height:auto;
    line-height:inherit;
    display:flex;
    justify-content:center;
    align-items:center;
    margin:5px;
    transition-duration:0.3s;
    transition-property:color, box-shadow, background, border;
    min-height:1rem;
    min-width:1rem;
  }
  .navbar1{
    display:flex;
    align-items:center;
    justify-content:space-between;
    width:98%;
    height:auto;
    padding:10px;
    max-width:1250px;
  }
  .navbar1 .simple-image-wrapper{
    width:8%;
  }
  .navbar1 .menu1-nav.menu-vertical{
    width:100% !important;
  }
  .navbar1-wrapper{
    width:100vw;
    min-height:50px;
    top:0px;
    display:flex;
    justify-content:center;
  }
  .short-animate{
    -webkit-transition:.5s ease-in-out;
    -moz-transition:.5s ease-in-out;
    -ms-transition:.5s ease-in-out;
    -o-transition:.5s ease-in-out;
    transition:.5s ease-in-out;
  }
  .lightbox{
    position:fixed;
    display:flex;
    background:rgba(0, 0, 0, 0.2);
    z-index:501;
    opacity:0;
    width:100%;
  }
  .lightbox-controls{
    display:block;
    position:absolute;
    overflow:hidden;
    z-index:502;
    width:fit-content;
  }
  .lightbox:target{
    top:0%;
    bottom:0%;
    opacity:1;
  }
  .lightbox:target ~  lightbox-controls{
    top:0px;
  }
  .gjs-row{
    position:relative;
    display:flex;
    flex-wrap:wrap;
    text-align:left;
    max-width:100%;
    width:100%;
    padding:10px;
  }
  .cell-1 > .gjs-cell{
    flex:auto;
  }
  .cell-2 > .gjs-cell{
    flex:1;
  }
  .cell-3 > .gjs-cell{
    flex:1;
  }
  .cell-4 > .gjs-cell{
    flex:1;
  }
  .gjs-cell{
    min-height:75px;
    position:relative;
    box-sizing:border-box;
  }
  .image-wrapper{
    display:flex;
    justify-content:center;
    width:100%;
    max-height:100%;
  }
  .gallery-lightboxes .image-lightbox{
    position:fixed;
    top:0;
    left:0;
    width:100vw;
    height:100vh;
    background:rgba(0,0,0,0.8);
    backdrop-filter:blur(5px);
    display:flex;
    align-items:center;
    justify-content:center;
    opacity:0;
    visibility:hidden;
    transition:opacity 0ms ease-in-out;
    z-index:11;
  }
  .gallery-lightboxes .image-lightbox:target{
    opacity:1;
    visibility:visible;
  }
  .gallery-lightboxes .image-lightbox:target .image-lightbox-wrapper{
    opacity:1;
    transform:scale(1,1) translateY(0);
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper{
    transform:scale(0.95,0.95) translateY(-30px);
    transition:opacity 500ms ease-in-out, transform 500ms ease-in-out;
    opacity:0;
    margin:1em auto;
    max-width:75%;
    padding:.5em;
    display:inline-block;
    background:#fff;
    box-shadow:0 0 5px rgba(0,0,0,0.8);
    position:relative;
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper .close{
    width:1.5em;
    height:1.5em;
    background:#000;
    color:#fff;
    font-weight:bold;
    text-decoration:none;
    border-radius:50%;
    box-shadow:0 0 0 2px white inset, 0 0 5px rgba(0, 0, 0, 0.5);
    position:absolute;
    right:-1em;
    top:-1em;
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper .close:before{
    content:'';
    display:block;
    width:10px;
    height:2px;
    background:#fff;
    margin:-1px 0 0 -5px;
    position:absolute;
    top:50%;
    left:50%;
    transform:rotate(-45deg);
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper .close:after{
    content:'';
    display:block;
    width:10px;
    height:2px;
    background:#fff;
    margin:-1px 0 0 -5px;
    position:absolute;
    top:50%;
    left:50%;
    transform:rotate(45deg);
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper .arrow-left{
    position:absolute;
    top:0;
    right:50%;
    bottom:0;
    left:0;
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper .arrow-left:before{
    content:'';
    display:inline-block;
    width:20px;
    height:20px;
    border:2px solid #fff;
    border-bottom:0;
    border-right:0;
    border-radius:4px 0 0 0;
    position:absolute;
    top:50%;
    right:100%;
    cursor:pointer;
    transform:rotate(-45deg) translateY(-50%);
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper .arrow-right{
    position:absolute;
    top:0;
    right:0;
    bottom:0;
    left:50%;
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper .arrow-right:before{
    content:'';
    display:block;
    width:20px;
    height:20px;
    border:2px solid #fff;
    border-bottom:0;
    border-left:0;
    border-radius:0 4px 0 0;
    position:absolute;
    top:50%;
    left:100%;
    cursor:pointer;
    transform:rotate(45deg) translateY(-50%);
  }
  .gallery-lightboxes .image-lightbox .image-lightbox-wrapper img{
    margin:0 auto;
    max-height:70vh;
    width:100%;
  }
  @media (max-width: 19200px){
    body, h1, h2, h3, h4, h5, h6, p, div, img, ul, li, ol, dl{
      margin-block-start:0px;
      margin-block-end:0px;
      margin-inline-start:0px;
      margin-inline-end:0px;
    }
    p, div.default-color, label{
      font-family:Overpass, Sans Serif;
      font-size:16px;
      font-weight:300;
      line-height:1.2;
      letter-spacing:normal;
      font-style:normal;
      color:#000000;
      text-decoration:inherit;
    }
    h1{
      font-family:montserrat;
      font-size:30px;
      font-weight:600;
      line-height:1.3;
      letter-spacing:normal;
      font-style:normal;
      color:#000000;
      text-decoration:inherit;
    }
    h2{
      font-family:montserrat;
      font-size:22px;
      font-weight:600;
      line-height:1.3;
      letter-spacing:normal;
      font-style:normal;
      color:#000000;
      text-decoration:inherit;
    }
    h3{
      font-family:montserrat;
      font-size:32px;
      font-weight:600;
      line-height:1.3;
      letter-spacing:normal;
      font-style:normal;
      color:#000000;
      text-decoration:inherit;
    }
    h4{
      font-family:montserrat;
      font-size:26px;
      font-weight:500;
      line-height:1.4;
      letter-spacing:normal;
      font-style:normal;
      color:#000000;
      text-decoration:inherit;
    }
    h5{
      font-family:montserrat;
      font-size:26px;
      font-weight:500;
      line-height:1.4;
      letter-spacing:normal;
      font-style:normal;
      color:#000000;
      text-decoration:inherit;
    }
    h6{
      font-family:montserrat;
      font-size:26px;
      font-weight:500;
      line-height:1.4;
      letter-spacing:normal;
      font-style:normal;
      color:#000000;
      text-decoration:inherit;
    }
    #ictk{
      min-height:50px;
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      justify-content:center;
      flex-grow:1;
      margin:0 0 0 0;
      width:100%;
      max-width:90%;
      padding:0px 10px;
    }
    #inz8{
      height:auto;
    }
    #i36p{
      flex-grow:0;
      height:0px;
    }
    #iwga{
      flex-grow:0;
    }
    #imu9{
      width:100vw;
      min-height:50px;
      top:0px;
      display:flex;
      justify-content:center;
      z-index:2;
    }
    #ilaoi{
      background-color:rgba(0, 0, 0, 0.3);
      justify-content:right;
      top:-100%;
      bottom:100%;
      left:0;
      right:0;
    }
    #iao5n{
      0:b;
      1:a;
      2:c;
      3:k;
      4:g;
      5:r;
      6:o;
      7:u;
      8:n;
      9:d;
      10:-;
      11:c;
      12:o;
      13:l;
      14:o;
      15:r;
      16::;
      17:w;
      18:h;
      19:i;
      20:t;
      21:e;
      22:;
      ;
      23:a;
      24:l;
      25:i;
      26:g;
      27:n;
      28:-;
      29:s;
      30:e;
      31:l;
      32:f;
      33::;
      34:c;
      35:e;
      36:n;
      37:t;
      38:e;
      39:r;
      40:;
      ;
      41:m;
      42:i;
      43:n;
      44:-;
      45:w;
      46:i;
      47:d;
      48:t;
      49:h;
      50::;
      51:5;
      52:%;
      53:;
      ;
      54:m;
      55:a;
      56:x;
      57:-;
      58:h;
      59:e;
      60:i;
      61:g;
      62:h;
      63:t;
      64::;
      65:c;
      66:a;
      67:l;
      68:c;
      69:(;
      70:1;
      71:0;
      72:0;
      73:v;
      74:h;
      75: ;
      76:-;
      77: ;
      78:6;
      79:0;
      80:p;
      81:x;
      82:);
      83:;
      ;
      84:h;
      85:e;
      86:i;
      87:g;
      88:h;
      89:t;
      90::;
      91:1;
      92:0;
      93:%;
      94:;
      ;
      95:m;
      96:i;
      97:n;
      98:-;
      99:h;
      100:e;
      101:i;
      102:g;
      103:h;
      104:t;
      105::;
      106:6;
      107:0;
      108:%;
      109:;
      ;
      110:f;
      111:l;
      112:e;
      113:x;
      114:-;
      115:d;
      116:i;
      117:r;
      118:e;
      119:c;
      120:t;
      121:i;
      122:o;
      123:n;
      124::;
      125:c;
      126:o;
      127:l;
      128:u;
      129:m;
      130:n;
      131:;
      ;
      132:j;
      133:u;
      134:s;
      135:t;
      136:i;
      137:f;
      138:y;
      139:-;
      140:c;
      141:o;
      142:n;
      143:t;
      144:e;
      145:n;
      146:t;
      147::;
      148:f;
      149:l;
      150:e;
      151:x;
      152:-;
      153:s;
      154:t;
      155:a;
      156:r;
      157:t;
      158:;
      ;
      159:a;
      160:l;
      161:i;
      162:g;
      163:n;
      164:-;
      165:i;
      166:t;
      167:e;
      168:m;
      169:s;
      170::;
      171:s;
      172:t;
      173:r;
      174:e;
      175:t;
      176:c;
      177:h;
      178:;
      ;
      179:o;
      180:v;
      181:e;
      182:r;
      183:f;
      184:l;
      185:o;
      186:w;
      187::;
      188:h;
      189:i;
      190:d;
      191:d;
      192:e;
      193:n;
      194:;
      ;
      195:d;
      196:i;
      197:s;
      198:p;
      199:l;
      200:a;
      201:y;
      202::;
      203:f;
      204:l;
      205:e;
      206:x;
      207:;
      ;
      208:w;
      209:i;
      210:d;
      211:t;
      212:h;
      213::;
      214:1;
      215:0;
      216:0;
      217:%;
      218:;
      ;
      219:m;
      220:a;
      221:x;
      222:-;
      223:w;
      224:i;
      225:d;
      226:t;
      227:h;
      228::;
      229:8;
      230:0;
      231:%;
      232:;
      ;
      233:p;
      234:o;
      235:s;
      236:i;
      237:t;
      238:i;
      239:o;
      240:n;
      241::;
      242:r;
      243:e;
      244:l;
      245:a;
      246:t;
      247:i;
      248:v;
      249:e;
      250:;
      ;
      background-color:white;
      align-self:center;
      min-width:5%;
      max-height:100vh;
      height:100%;
      min-height:60%;
      flex-direction:column;
      justify-content:flex-start;
      align-items:stretch;
      overflow:hidden;
      display:flex;
      width:55%;
      max-width:80%;
      position:relative;
    }
    #i01lx{
      top:0;
      right:0;
      position:absolute;
      cursor:pointer;
    }
    #iohrd{
      color:#0dacff;
      text-decoration:none;
      text-align:center;
      height:auto;
      line-height:inherit;
      display:flex;
      justify-content:center;
      align-items:center;
      margin:5px;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      font-size:24px;
    }
    #ic4oh{
      width:100%;
      height:100%;
      flex-direction:inherit;
      justify-content:inherit;
      align-items:inherit;
      display:flex;
      overflow:auto;
      position:relative;
    }
    #inzkg{
      z-index:11;
    }
    #ijk5t{
      width:initial;
    }
    #i3efx{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #imnai{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #i7mgp{
      width:initial;
    }
    #i0ju2{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #ibdlx{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #isdpe{
      width:initial;
    }
    #imxfwa{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #ijwg01{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #iquq46{
      width:initial;
    }
    #i6lkog{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #ilhw28{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #iwf10k{
      width:initial;
    }
    #inzkg.menu-vertical ul li:hover > ul li{
      background-color:#0dacff;
    }
    #i1znl{
      0:c;
      1:o;
      2:l;
      3:o;
      4:r;
      5::;
      6:#;
      7:0;
      8:d;
      9:a;
      10:c;
      11:f;
      12:f;
      13:;
      ;
      14:t;
      15:e;
      16:x;
      17:t;
      18:-;
      19:d;
      20:e;
      21:c;
      22:o;
      23:r;
      24:a;
      25:t;
      26:i;
      27:o;
      28:n;
      29::;
      30:n;
      31:o;
      32:n;
      33:e;
      34:;
      ;
      35:d;
      36:i;
      37:s;
      38:p;
      39:l;
      40:a;
      41:y;
      42::;
      43:n;
      44:o;
      45:n;
      46:e;
      47:;
      ;
      color:#0dacff;
      text-decoration:none;
      display:none;
      font-size:24px;
    }
    #ih2rh{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:9%;
      padding-top:6%;
      position:relative;
      min-height:20px;
    }
    #ilavk{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #iv2gl{
      object-fit:contain;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #iumhd{
      height:auto;
    }
    #iqy1f{
      width:auto;
    }
    #isjjl{
      z-index:11;
    }
    #ite95{
      width:initial;
    }
    #i1lv7{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #ijxdy{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #ii1p6{
      width:initial;
    }
    #inrxu{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #iy1qg{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #im3sm{
      width:initial;
    }
    #i5uwv{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #iap3m{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #i97jw{
      width:initial;
    }
    #iepmh{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #ib6gg{
      color:#0dacff;
      text-decoration:none;
      font-size:16px;
    }
    #i6wrv{
      width:initial;
    }
    #isjjl.menu-vertical ul li:hover > ul li{
      background-color:#0dacff;
    }
    #ie6q5g{
      width:100%;
    }
    #iv1rkk{
      grid-row-gap:10px;
      grid-column-gap:10px;
      margin:auto;
    }
    #id1jpo{
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      max-width:100%;
      width:100%;
    }
    #id3795{
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      max-width:100%;
      width:100%;
    }
    #ibaq19{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
    }
    #i4dujx{
      width:initial;
    }
    #i0zhag{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
    }
    #imjg91{
      width:initial;
    }
    #i27xlo{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:67.8%;
      padding-top:47%;
      position:relative;
    }
    #ihlrni{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #in4ejs{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #it72yz{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:24.49%;
      padding-top:15%;
      position:relative;
      border-color:#ffffff;
      border-style:none;
      border-width:0px;
      border-radius:0px 0px 0px 0px;
    }
    #iv8nua{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #iahyty{
      object-fit:contain;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #iy739s{
      height:auto;
    }
    #io2d4r{
      min-height:50px;
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      justify-content:center;
      flex-grow:1;
      margin:0 0 0 0;
      width:100%;
      max-width:90%;
      padding:0px 10px;
    }
    #iivxau{
      height:auto;
    }
    #izlecb{
      flex-grow:0;
    }
    #ibf6qk{
      flex-grow:0;
    }
    #ijpkuq{
      display:none;
    }
    #i35pjj{
      min-height:50px;
      position:relative;
      width:100%;
      height:auto;
      overflow:hidden;
      max-width:100%;
      margin:24px 24px 24px 24px;
      padding:24px 24px 24px 24px;
    }
    #ip1ogt{
      margin-bottom:20px;
    }
    #ij0zk7{
      padding:5px 0;
      min-height:100px;
    }
    #ipf8qn{
      width:100%;
      overflow:hidden;
    }
    #iz7l6j{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:100%;
      padding-top:70%;
      position:relative;
    }
    #i4zzfx{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #i2na1l{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #ilgl1y{
      padding:5px 0;
      min-height:100px;
    }
    #i5p303{
      width:100%;
      overflow:hidden;
    }
    #ifme1l{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:100%;
      padding-top:70%;
      position:relative;
    }
    #ia7fbg{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #i8tf3s{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #i82fp8{
      padding:5px 0;
      min-height:100px;
    }
    #ihkb2h{
      width:100%;
      overflow:hidden;
    }
    #icf8uq{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:100%;
      padding-top:70%;
      position:relative;
    }
    #iom3ol{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #iq6tbk{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #it212h{
      padding:5px 0;
      min-height:100px;
    }
    #iizpsz{
      width:100%;
      overflow:hidden;
    }
    #i1cevt{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:100%;
      padding-top:70%;
      position:relative;
    }
    #iaqc0r{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #ia8squ{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #itc3sa{
      padding:5px 0;
      min-height:100px;
    }
    #iitmsf{
      width:100%;
      overflow:hidden;
    }
    #ilf1rc{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:100%;
      padding-top:70%;
      position:relative;
    }
    #ibn9cv{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #ifny0n{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #i6vlck{
      color:#0dacff;
    }
    #iq7knd{
      color:#0dacff;
    }
    #idj3yh{
      --swiper-pagination-color:#0dacff;
      --swiper-pagination-bullet-inactive-color:#8e8e8e;
    }
    #i1o8yg{
      padding:5px 0;
      min-height:100px;
    }
    #iyglsq{
      width:100%;
      overflow:hidden;
    }
    #iehjwl{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:100%;
      padding-top:70%;
      position:relative;
    }
    #i10d4x{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #iwxi4f{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #iu2n7h{
      width:100%;
    }
    #iwn90d{
      grid-row-gap:10px;
      grid-column-gap:10px;
      margin:auto;
    }
    #ic7sgx{
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      max-width:100%;
      width:100%;
    }
    #ivuvfn{
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      max-width:100%;
      width:100%;
    }
    #i5bayn{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
    }
    #ic61p5{
      width:initial;
    }
    #ijm4lj{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
    }
    #ieo1ni{
      width:initial;
    }
    #istyx6{
      width:100%;
    }
    #ipe5b2{
      grid-row-gap:10px;
      grid-column-gap:10px;
      margin:auto;
    }
    #itc106{
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      max-width:100%;
      width:100%;
    }
    #i9ycsj{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:19.98%;
      padding-top:14%;
      position:relative;
    }
    #idwe4x{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #iegwss{
      object-fit:contain;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #iq77sa{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
    }
    #ib5umm{
      width:initial;
    }
    #iwacum{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
      width:341.672px;
    }
    #iop0sg{
      width:initial;
    }
    #iazsfz{
      object-fit:cover;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #itjjw1{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #i5dsn4{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:19.98%;
      padding-top:14%;
      position:relative;
    }
    #inuh6k{
      width:initial;
    }
    #i562dz{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
    }
    #i562dz p{
      margin-top:auto;
      margin-bottom:auto;
    }
    #iqb8l9{
      width:initial;
    }
    #ii39tj{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
      width:341.672px;
    }
    #ii39tj p{
      margin-top:auto;
      margin-bottom:auto;
      width:341.672px;
    }
    #i0je5v{
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      max-width:100%;
      width:100%;
    }
    #imblvi{
      object-fit:contain;
      width:100%;
      height:100%;
      background-color:transparent;
      object-position:50% 50%;
      margin-left:0px;
      margin-top:0px;
    }
    #i9ueop{
      width:100%;
      height:100%;
      position:absolute;
      top:0px;
    }
    #iaazko{
      display:flex;
      justify-content:center;
      width:100%;
      overflow:hidden;
      margin:0px;
      max-width:19.98%;
      padding-top:14%;
      position:relative;
    }
    #io9jn1{
      width:initial;
    }
    #icwr0h{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
    }
    #icwr0h p{
      margin-top:auto;
      margin-bottom:auto;
    }
    #i0wjhg{
      width:initial;
    }
    #ixzz64{
      display:block;
      justify-content:center;
      align-self:center;
      text-align:center;
      transition-duration:0.3s;
      transition-property:color, box-shadow, background, border;
      flex-basis:content;
      max-width:100%;
      margin-top:auto;
      margin-bottom:auto;
      width:341.672px;
    }
    #ixzz64 p{
      margin-top:auto;
      margin-bottom:auto;
      width:341.672px;
    }
    #iz3b7i{
      height:auto;
      display:flex;
      flex-direction:column;
      align-items:center;
      max-width:100%;
      width:100%;
    }
    #i31zds{
      height:auto;
    }
    #ixtk5i{
      height:auto;
    }
  }
  @media (max-width: 768px){
    .navbar1{
      flex-wrap:wrap;
    }
    .navbar1 .menu1-wrapper{
      display:none;
    }
    .navbar1 .menu1-burger{
      display:block !important;
    }
    .gjs-row{
      flex-wrap:wrap;
    }
    .cell-2 > .gjs-cell{
      flex:auto;
    }
    .cell-3 > .gjs-cell{
      flex:auto;
    }
    .cell-4 > .gjs-cell{
      flex:auto;
    }
  }
  
  </style>
</head>
<body>
    <body id="ic1i">
        <section id="ihpj" class="crm-section section-wrapper">
          <div detect-type="section" id="iye6" class="crm-bg">
            <div detect-type="section" id="i182" class="crm-bg-image">
            </div>
            <div detect-type="section" class="crm-bg-color">
            </div>
          </div>
          <div draggable="false" id="inz8" class="crm-section-inner">
            <div draggable="false" id="i36p" class="crm-section-padding section-padding-draggable section-padding-start">
            </div>
            <div draggable="false" id="ictk" class="crm-container">
              <div id="imu9" class="navbar1-wrapper">
                <div id="iumhd" class="navbar1">
                  <div ft-target="" id="ih2rh" class="image-background">
                    <a id="ilavk"><picture>
                      <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                      <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                      <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                      <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                      <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                      <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                      <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                      <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="iv2gl" class="img-fluid"/>
                      </picture></a>
                  </div>
                  <div id="iqy1f" class="menu1-wrapper">
                    <nav id="isjjl" class="menu1-nav">
                      <ul id="ite95">
                        <li>
                          <a draggable="false" href="" ft-popup=""><p>Home
                            </p><i target="" id="i1lv7" class="menu-icon up fas fa-angle-up">
                            </i><i target="" id="ijxdy" class="menu-icon down fas fa-angle-down">
                            </i></a>
                          <ul id="ii1p6">
                            <li>
                              <a draggable="false" href="" ft-popup=""><p>Home 1
                                </p><i target="" id="inrxu" class="menu-icon up fas fa-angle-up">
                                </i><i target="" id="iy1qg" class="menu-icon down fas fa-angle-down">
                                </i></a>
                              <ul id="im3sm">
                                <li>
                                  <a draggable="false" href="" ft-popup=""><p>Visit us
                                    </p></a>
                                </li>
                              </ul>
                            </li>
                            <li>
                              <a draggable="false" href="https://www.google.com" ft-popup=""><p>Support
                                </p></a>
                            </li>
                          </ul>
                        </li>
                        <li>
                          <a draggable="false" href="https://www.google.com" ft-popup=""><p>Features
                            </p></a>
                        </li>
                        <li>
                          <a draggable="false" href="" ft-popup=""><p>Services
                            </p><i target="" id="i5uwv" class="menu-icon up fas fa-angle-up">
                            </i><i target="" id="iap3m" class="menu-icon down fas fa-angle-down">
                            </i></a>
                          <ul id="i97jw">
                            <li>
                              <a draggable="false" href="" ft-popup=""><p>Visit
                                </p><i target="" id="iepmh" class="menu-icon up fas fa-angle-up">
                                </i><i target="" id="ib6gg" class="menu-icon down fas fa-angle-down">
                                </i></a>
                              <ul id="i6wrv">
                                <li>
                                  <a draggable="false" href="" ft-popup=""><p>Visit us 2
                                    </p></a>
                                </li>
                              </ul>
                            </li>
                            <li>
                              <a draggable="false" href="https://www.google.com" ft-popup=""><p>Support 2
                                </p></a>
                            </li>
                          </ul>
                        </li>
                        <li>
                          <a draggable="false" href="" ft-popup=""><p>Account
                            </p></a>
                        </li>
                      </ul>
                    </nav>
                  </div>
                  <i target="" ft-popup="ilaoi" id="i1znl" class="menu1-burger fas fa-bars">
                  </i>
                </div>
              </div>
            </div>
            <div ft-change-transition="top" ft-navbar-popup="iumhd" id="ilaoi" class="popup-wrapper lightbox short-animate">
              <div ft-show-position="right" ft-icon-position="topRight" id="iao5n" class="popup">
                <a id="i01lx" class="lightbox-controls"><i target="" id="iohrd" class="fas fa-times">
                  </i></a>
                <div id="ic4oh" class="popup-inner">
                  <nav id="inzkg" class="menu1-nav menu-vertical">
                    <ul id="ijk5t">
                      <li>
                        <a draggable="false" href="" ft-popup=""><p>Home
                          </p><i target="" id="i3efx" class="menu-icon up fas fa-angle-up">
                          </i><i target="" id="imnai" class="menu-icon down fas fa-angle-down">
                          </i></a>
                        <ul id="i7mgp">
                          <li>
                            <a draggable="false" href="" ft-popup=""><p>Home 1
                              </p><i target="" id="i0ju2" class="menu-icon up fas fa-angle-up">
                              </i><i target="" id="ibdlx" class="menu-icon down fas fa-angle-down">
                              </i></a>
                            <ul id="isdpe">
                              <li>
                                <a draggable="false" href="" ft-popup=""><p>Visit us
                                  </p></a>
                              </li>
                            </ul>
                          </li>
                          <li>
                            <a draggable="false" href="https://www.google.com" ft-popup=""><p>Support
                              </p></a>
                          </li>
                        </ul>
                      </li>
                      <li>
                        <a draggable="false" href="https://www.google.com" ft-popup=""><p>Features
                          </p></a>
                      </li>
                      <li>
                        <a draggable="false" href="" ft-popup=""><p>Services
                          </p><i target="" id="imxfwa" class="menu-icon up fas fa-angle-up">
                          </i><i target="" id="ijwg01" class="menu-icon down fas fa-angle-down">
                          </i></a>
                        <ul id="iquq46">
                          <li>
                            <a draggable="false" href="" ft-popup=""><p>Visit
                              </p><i target="" id="i6lkog" class="menu-icon up fas fa-angle-up">
                              </i><i target="" id="ilhw28" class="menu-icon down fas fa-angle-down">
                              </i></a>
                            <ul id="iwf10k">
                              <li>
                                <a draggable="false" href="" ft-popup=""><p>Visit us 2
                                  </p></a>
                              </li>
                            </ul>
                          </li>
                          <li>
                            <a draggable="false" href="https://www.google.com" ft-popup=""><p>Support 2
                              </p></a>
                          </li>
                        </ul>
                      </li>
                      <li>
                        <a draggable="false" href="" ft-popup=""><p>Account
                          </p></a>
                      </li>
                    </ul>
                  </nav>
                </div>
              </div>
              <div detect-type="popup-wrapper" id="iqzas" class="crm-bg">
                <div detect-type="popup-wrapper" class="crm-bg-image">
                </div>
                <div detect-type="popup-wrapper" class="crm-bg-color">
                </div>
              </div>
            </div>
            <div draggable="false" id="iwga" class="crm-section-padding section-padding-draggable section-padding-end">
            </div>
          </div>
        </section>
        <div id="ie6q5g" class="crm-grid-wrapper">
          <div ColumnGap="10px" RowGap="10px" id="iv1rkk" class="gjs-row cell-2">
            <div ColumnGap="10px" RowGap="10px" id="id1jpo" class="gjs-cell">
              <div id="ibaq19" class="crm-text">
                <h1 id="i4dujx">
                  <br/>Leading Blockchain Development Services
                </h1>
              </div>
              <div id="i0zhag" class="crm-text">
                <h2 id="imjg91">
                  <br/>One-stop solution for all your blockchain development needs. Smart contracts (ERC-20/ERC-721), DAPPs, ICO/IDOs, Launchpads, and more. Customised Solutions for every need.
                </h2>
              </div>
              <div id="iy739s" class="image-wrapper">
                <div ft-target="" id="it72yz" class="image-background">
                  <a id="iv8nua"><picture>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                    <img loading="eager" src="/assets/aws/st_e7n4k0/site_juv1l4/assets/icon-4c4bc7d4b28d87e81a7ca_pwvL80BF.gif" id="iahyty" class="img-fluid"/>
                    </picture></a>
                </div>
              </div>
            </div>
            <div ColumnGap="10px" RowGap="10px" id="id3795" class="gjs-cell">
              <div class="image-wrapper">
                <div ft-target="" id="i27xlo" class="image-background">
                  <a id="ihlrni"><picture>
                    <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="https://i.stack.imgur.com/y9DpT.jpg" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                    <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="in4ejs" class="img-fluid"/>
                    </picture></a>
                </div>
              </div>
            </div>
          </div>
        </div>
        <section class="crm-section section-wrapper" id="izmmdz">
          <div detect-type="section" id="igenna" class="crm-bg">
            <div detect-type="section" class="crm-bg-image" id="ie0n7l">
            </div>
            <div detect-type="section" class="crm-bg-color">
            </div>
          </div>
          <div draggable="false" class="crm-section-inner" id="iivxau">
            <div draggable="false" class="crm-section-padding section-padding-draggable section-padding-start" id="izlecb">
            </div>
            <div draggable="false" class="crm-container" id="io2d4r">
              <div id="i35pjj" class="swiper-container mySwiper">
                <div class="swiper-wrapper" id="ip1ogt">
                  <div class="swiper-slide" id="ij0zk7">
                    <div class="image-wrapper" id="ipf8qn">
                      <div ft-target="" class="image-background" id="iz7l6j">
                        <a id="i4zzfx"><picture>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download3_vCNhxiPW.png?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download3_vCNhxiPW.png?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download3_vCNhxiPW.png?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download3_vCNhxiPW.png?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download3_vCNhxiPW.png?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download3_vCNhxiPW.png?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download3_vCNhxiPW.png?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                          <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="i2na1l" class="img-fluid"/>
                          </picture></a>
                      </div>
                    </div>
                  </div>
                  <div class="swiper-slide" id="ilgl1y">
                    <div class="image-wrapper" id="i5p303">
                      <div ft-target="" class="image-background" id="ifme1l">
                        <a id="ia7fbg"><picture>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download4_i2KIzOLP.png?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download4_i2KIzOLP.png?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download4_i2KIzOLP.png?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download4_i2KIzOLP.png?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download4_i2KIzOLP.png?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download4_i2KIzOLP.png?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download4_i2KIzOLP.png?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                          <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="i8tf3s" class="img-fluid"/>
                          </picture></a>
                      </div>
                    </div>
                  </div>
                  <div class="swiper-slide" id="i82fp8">
                    <div class="image-wrapper" id="ihkb2h">
                      <div ft-target="" class="image-background" id="icf8uq">
                        <a id="iom3ol"><picture>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images1_IzNBh7Tp.png?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images1_IzNBh7Tp.png?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images1_IzNBh7Tp.png?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images1_IzNBh7Tp.png?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images1_IzNBh7Tp.png?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images1_IzNBh7Tp.png?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images1_IzNBh7Tp.png?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                          <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="iq6tbk" class="img-fluid"/>
                          </picture></a>
                      </div>
                    </div>
                  </div>
                  <div class="swiper-slide" id="it212h">
                    <div class="image-wrapper" id="iizpsz">
                      <div ft-target="" class="image-background" id="i1cevt">
                        <a id="iaqc0r"><picture>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images4_IA7t1noM.jfif?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images4_IA7t1noM.jfif?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images4_IA7t1noM.jfif?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images4_IA7t1noM.jfif?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images4_IA7t1noM.jfif?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images4_IA7t1noM.jfif?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images4_IA7t1noM.jfif?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                          <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="ia8squ" class="img-fluid"/>
                          </picture></a>
                      </div>
                    </div>
                  </div>
                  <div class="swiper-slide" id="itc3sa">
                    <div class="image-wrapper" id="iitmsf">
                      <div ft-target="" class="image-background" id="ilf1rc">
                        <a id="ibn9cv"><picture>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download6_WkGnvwHr.png?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download6_WkGnvwHr.png?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download6_WkGnvwHr.png?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download6_WkGnvwHr.png?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download6_WkGnvwHr.png?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download6_WkGnvwHr.png?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download6_WkGnvwHr.png?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                          <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="ifny0n" class="img-fluid"/>
                          </picture></a>
                      </div>
                    </div>
                  </div>
                  <div class="swiper-slide" id="i1o8yg">
                    <div class="image-wrapper" id="iyglsq">
                      <div ft-target="" class="image-background" id="iehjwl">
                        <a id="i10d4x"><picture>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download5_P78Vnbw4.png?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download5_P78Vnbw4.png?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download5_P78Vnbw4.png?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download5_P78Vnbw4.png?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download5_P78Vnbw4.png?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download5_P78Vnbw4.png?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                          <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download5_P78Vnbw4.png?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                          <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="iwxi4f" class="img-fluid"/>
                          </picture></a>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="swiper-button-prev" id="i6vlck">
                </div>
                <div class="swiper-button-next" id="iq7knd">
                </div>
                <div class="swiper-pagination" id="idj3yh">
                </div>
                <div class="swiper-scrollbar" id="ijpkuq">
                </div>
              </div>
            </div>
            <div draggable="false" class="crm-section-padding section-padding-draggable section-padding-end" id="ibf6qk">
            </div>
          </div>
        </section>
        <div class="crm-grid-wrapper" id="iu2n7h">
          <div ColumnGap="10px" RowGap="10px" class="gjs-row cell-2" id="iwn90d">
            <div ColumnGap="10px" RowGap="10px" class="gjs-cell" id="ic7sgx">
              <div class="crm-text" id="ijm4lj">
                <h1 id="ieo1ni">
                  <br/>KWS has a dynamic team of blockchain, frontend &amp; backend developers.
                </h1>
              </div>
            </div>
            <div ColumnGap="10px" RowGap="10px" class="gjs-cell" id="ivuvfn">
              <div class="crm-text" id="i5bayn">
                <h2 id="ic61p5">We take care of all your token launch needs. Creation of UI/UX and landing page for your token, Smart Contract, ICO/IDO launchpad, NFT Minting &amp; Marketplace, various DAPPs, and more.
                </h2>
              </div>
            </div>
          </div>
        </div>
        <div class="crm-grid-wrapper" id="istyx6">
          <div ColumnGap="10px" RowGap="10px" class="gjs-row cell-3" id="ipe5b2">
            <div ColumnGap="10px" RowGap="10px" class="gjs-cell" id="itc106">
              <div class="image-wrapper" id="i31zds">
                <div ft-target="" class="image-background" id="i9ycsj">
                  <a id="idwe4x"><picture>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download7_LxTWPqEb.png?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download7_LxTWPqEb.png?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download7_LxTWPqEb.png?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download7_LxTWPqEb.png?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download7_LxTWPqEb.png?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download7_LxTWPqEb.png?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/download7_LxTWPqEb.png?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                    <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="iegwss" class="img-fluid"/>
                    </picture></a>
                </div>
              </div>
              <div class="crm-text" id="iq77sa">
                <h2 id="ib5umm">100% Legit
                </h2>
              </div>
              <div class="crm-text" id="iwacum">
                <p id="iop0sg">The volume of work we deliver each month speaks for itself. We have delivered high quality DeFi services.
                </p>
              </div>
            </div>
            <div ColumnGap="10px" RowGap="10px" class="gjs-cell" id="iz3b7i">
              <div class="image-wrapper" id="ixtk5i">
                <div ft-target="" class="image-background" id="iaazko">
                  <a id="i9ueop"><picture>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images2_r8ofg1yL.png?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images2_r8ofg1yL.png?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images2_r8ofg1yL.png?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images2_r8ofg1yL.png?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images2_r8ofg1yL.png?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images2_r8ofg1yL.png?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images2_r8ofg1yL.png?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                    <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="imblvi" class="img-fluid"/>
                    </picture></a>
                </div>
              </div>
              <div class="crm-text" id="icwr0h">
                <h2 id="io9jn1">Escrow Payments
                </h2>
              </div>
              <div class="crm-text" id="ixzz64">
                <p id="i0wjhg">We believe in transparency. We offer escrow payment options to our clients.
                  <br/>
                </p>
              </div>
            </div>
            <div ColumnGap="10px" RowGap="10px" class="gjs-cell" id="i0je5v">
              <div class="image-wrapper">
                <div ft-target="" class="image-background" id="i5dsn4">
                  <a id="itjjw1"><picture>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images5_6vx2pE8e.jfif?width=1280" media="(min-width: 1401px), (min-width:769px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images5_6vx2pE8e.jfif?width=1280" media="(min-width:1025px) and (max-width:1400px), (min-width:577px) and (max-width:768px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images5_6vx2pE8e.jfif?width=1024" media="(min-width:769px) and (max-width:1024px), (min-width:361px) and (max-width:576px) and (-webkit-min-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images5_6vx2pE8e.jfif?width=720" media="(min-width:577px) and (max-width:768px), (min-width:361px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images5_6vx2pE8e.jfif?width=576" media="(max-width:421px) and (max-width:576px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images5_6vx2pE8e.jfif?width=420" media="(max-width:361px) and (max-width:420px) and (-webkit-max-device-pixel-ratio: 1.9)" type="image/webp"/>
                    <source srcset="/assets/aws/st_e7n4k0/site_juv1l4/assets/images5_6vx2pE8e.jfif?width=360" media="(max-width:360px) and (-webkit-max-device-pixel-ratio: 3.0)" type="image/webp"/>
                    <img loading="eager" src="https://i.stack.imgur.com/y9DpT.jpg" id="iazsfz" class="img-fluid"/>
                    </picture></a>
                </div>
              </div>
              <div class="crm-text" id="i562dz">
                <h2 id="inuh6k">Consultation &amp; Support
                </h2>
              </div>
              <div class="crm-text" id="ii39tj">
                <p id="iqb8l9">Our team of experts will guide you throughout the life of your projects.
                </p>
              </div>
            </div>
          </div>
        </div>
      </body>
      <script>var props = {
          "iye6":{
            "stylePrefix":"crm-"}
          ,"iqzas":{
            "stylePrefix":"crm-"}
          ,"igenna":{
            "stylePrefix":"crm-"}
        };
        var ids = Object.keys(props).map(function(id) {
          return '#'+id }
                                        ).join(',');
        var els = document.querySelectorAll(ids);
        for (var i = 0, len = els.length; i < len; i++) {
          var el = els[i];
          (function(t){
            var e=t.stylePrefix,n=document.getElementById("".concat(e,"background-style"));
            if(!n){
              var r="\n                .".concat(e,"bg{\n                    position: absolute;\n                    top: 0;\n                    left: 0;\n                    width: 100%;\n                    height: 100%;\n                    z-index:-1;\n                }\n                .").concat(e,"bg-color{\n                    position: absolute;\n                    top: 0;\n                    left: 0;\n                    width: 100%;\n                    height: 100%;\n                }\n                .").concat(e,"bg-image{\n                    position: absolute;\n                    top: 0;\n                    left: 0;\n                    width: 100%;\n                    height: 100%;\n                    background-repeat: no-repeat;\n                    background-size: cover;\n                }\n                .").concat(e,"bg-video{\n                    position: absolute;\n                    top: 0;\n                    left: 0;\n                    width: 100%;\n                    height: 100%;\n                }\n            ");
              (n=document.createElement("style")).id="".concat(e,"background-style"),n.type="text/css",n.styleSheet?n.styleSheet.cssText=r:n.appendChild(document.createTextNode(r)),document.head.appendChild(n)}
          }
           .bind(el))(props[el.id]);
        }
        var items = document.querySelectorAll('#iumhd');
        for (var i = 0, len = items.length; i < len; i++) {
          (function(){
            var t=this.querySelector(".menu1-burger");
            if(t){
              var e=t.getAttribute("ft-popup");
              if(e){
                var n=document.getElementById(e);
                if(n)for(var r=n.querySelector(".popup"),o=function(){
                  if(r){
                    var t=n.getAttribute("ft-change-transition");
                    setTimeout((function(){
                      "top"===t?(n.style.top="-100%",n.style.bottom="100%"):"right"===t?(n.style.left="100%",n.style.right="-100%"):"bottom"===t?(n.style.top="100%",n.style.bottom="-100%"):"left"===t&&(n.style.left="-100%",n.style.right="100%"),n.style.opacity="0"}
                               ),50),setTimeout((function(){
                      r.style.display="none"}
                                                ),250)}
                }
                         ,i=n.querySelectorAll(".menu-vertical ul li"),a=0;a<i.length;a++)i[a].addEventListener("click",(function(t){
                  o()}
                                                                                                                        ))}
            }
          }
           .bind(items[i]))();
        }
        var props = {
          "i1lv7":{
          }
          ,"ijxdy":{
          }
          ,"inrxu":{
          }
          ,"iy1qg":{
          }
          ,"i5uwv":{
          }
          ,"iap3m":{
          }
          ,"iepmh":{
          }
          ,"ib6gg":{
          }
          ,"i1znl":{
          }
          ,"iohrd":{
          }
          ,"i3efx":{
          }
          ,"imnai":{
          }
          ,"i0ju2":{
          }
          ,"ibdlx":{
          }
          ,"imxfwa":{
          }
          ,"ijwg01":{
          }
          ,"i6lkog":{
          }
          ,"ilhw28":{
          }
        };
        var ids = Object.keys(props).map(function(id) {
          return '#'+id }
                                        ).join(',');
        var els = document.querySelectorAll(ids);
        for (var i = 0, len = els.length; i < len; i++) {
          var el = els[i];
          (function m(){
            var t=this,e=function(){
              t.parentNode.parentNode.children[1].classList.contains("navbar-menu-hidden")?(t.parentNode.parentNode.style.height="100vh",t.parentNode.parentNode.children[1].classList.remove("navbar-menu-hidden"),t.parentNode.parentNode.children[1].style.width="100%",t.parentNode.parentNode.children[1].style.height="100%",t.parentNode.parentNode.children[1].style.overflow="visible",t.classList.remove("fa-bars"),t.classList.add("fa-times")):function(){
                var e=t.parentNode.parentNode.style;
                delete e.height,delete e.width;
                var n=t.parentNode.getBoundingClientRect(),r=n&&n.height?n.height:"5rem";
                t.parentNode.parentNode.children[1].classList.add("navbar-menu-hidden"),t.parentNode.parentNode.children[1].style=e,t.parentNode.parentNode.children[1].style.overflow="hidden",t.parentNode.parentNode.style.height=r,t.classList.add("fa-bars"),t.classList.remove("fa-times")}
              ()};
            t.parentNode&&t.parentNode.parentNode&&t.parentNode.parentNode.children&&t.parentNode.parentNode.children[1]&&t.parentNode.parentNode.children[1].classList.contains("navbar-menu-vertical")&&t.addEventListener("click",e),"1"!==this.getAttribute("data-design-mode")&&this.addEventListener("click",(function(e){
              if(t.getAttribute("ft-popup")){
                e.preventDefault();
                var n=document.getElementById(t.getAttribute("ft-popup")),r=n.getElementsByClassName("popup")[0],o=n.getAttribute("ft-change-transition");
                "top"===o||"bottom"===o?(n.style.top="0%",n.style.bottom="0%"):"right"!==o&&"left"!==o||(n.style.left="0%",n.style.right="0%"),n.style.display="flex",n.style.opacity="1",r.style.display="flex"}
            }
      ))}
           .bind(el))(props[el.id]);
        }
        var items = document.querySelectorAll('#ilaoi');
        for (var i = 0, len = items.length; i < len; i++) {
          (function(){
            var t=this;
            "1"!=this.getAttribute("data-design-mode")&&this.addEventListener("click",(function(e){
              !function(){
                var e=t,n=e.querySelector(".popup");
                console.log("wrapper",e,n);
                var r=e.getAttribute("ft-change-transition");
                setTimeout((function(){
                  "top"===r?(e.style.top="-100%",e.style.bottom="100%"):"right"===r?(e.style.left="100%",e.style.right="-100%"):"bottom"===r?(e.style.top="100%",e.style.bottom="-100%"):"left"===r&&(e.style.left="-100%",e.style.right="100%"),e.style.opacity="0",console.log("wrapper 2",e,e.style)}
                           ),50),setTimeout((function(){
                  n&&(n.style.display="none")}
                                            ),250)}
              ()}
                                                                                      ))
          }
           .bind(items[i]))();
        }
        var items = document.querySelectorAll('#iao5n');
        for (var i = 0, len = items.length; i < len; i++) {
          (function(){
            var t=this;
            "1"!=t.getAttribute("data-design-mode")&&this.addEventListener("click",(function(t){
              console.log("popup click",t),t.target,t.cancelBubble=!0}
                                                                                   ))
          }
           .bind(items[i]))();
        }
        var props = {
          "i01lx":{
          }
        };
        var ids = Object.keys(props).map(function(id) {
          return '#'+id }
                                        ).join(',');
        var els = document.querySelectorAll(ids);
        for (var i = 0, len = els.length; i < len; i++) {
          var el = els[i];
          (function dl(t){
            var e=this,n=this.parentNode.parentNode,r=n.getElementsByClassName("popup"),o=r.length>0?r[0]:null;
            e.addEventListener("click",(function(){
              if(o){
                console.log("closePopup",e);
                var t=n.getAttribute("ft-change-transition");
                setTimeout((function(){
                  "top"===t?(n.style.top="-100%",n.style.bottom="100%"):"right"===t?(n.style.left="100%",n.style.right="-100%"):"bottom"===t?(n.style.top="100%",n.style.bottom="-100%"):"left"===t&&(n.style.left="-100%",n.style.right="100%"),n.style.opacity="0"}
                           ),50),setTimeout((function(){
                  o.style.display="none"}
                                            ),250)}
            }
                                       ))}
           .bind(el))(props[el.id]);
        }
        var props = {
          "i35pjj":{
            "script-deps":"https://cdnjs.cloudflare.com/ajax/libs/Swiper/8.0.5/swiper-bundle.min.js","style-deps":"https://cdnjs.cloudflare.com/ajax/libs/Swiper/8.0.5/swiper-bundle.min.css","enabled":true,"preventClicks":true,"initialSlide":"0","speed":300,"allowTouchMove":false,"slidesPerView":4,"spaceBetween":"40","slidesPerGroup":1,"slidesOffsetBefore":"0","slidesOffsetAfter":"0","direction":"horizontal","effect":"slide","autoHeight":false,"watchOverflow":true,"centeredSlides":false,"autoplay":false,"disableOnInteraction":true,"loop":false,"freeMode":false,"minimumVelocity":0.02,"momentum":true,"keyboard":false,"mousewheel":false,"ft-slides-1200":4,"ft-space-1200":"40","ft-perGroup-1200":1,"pagination":"none","dynamicBullets":false,"progressbarOpposite":false,"autoplayDelay":3000,"autoplayStopOnLastSlide":false,"autoplayDisableOnInteraction":true,"autoplayReverseDirection":false,"autoplayWaitForTransition":true,"scrollbar":false}
        };
        var ids = Object.keys(props).map(function(id) {
          return '#'+id }
                                        ).join(',');
        var els = document.querySelectorAll(ids);
        for (var i = 0, len = els.length; i < len; i++) {
          var el = els[i];
          (function(t){
            var e,n=t["script-deps"],r=t["style-deps"],o=this.getAttribute("id"),i={
              enabled:!!t.enabled,preventClicks:!!t.preventClicks,initialSlide:parseInt(t.initialSlide,10),speed:parseInt(t.speed,10),observer:!0,grabCursor:!1,allowTouchMove:!!t.allowTouchMove,slidesPerView:parseInt(t.slidesPerView,10),spaceBetween:parseInt(t.spaceBetween,10),slidesPerGroup:parseInt(t.slidesPerGroup,10),slidesOffsetBefore:parseInt(t.slidesOffsetBefore,10),slidesOffsetAfter:parseInt(t.slidesOffsetAfter,10),direction:t.direction,effect:t.effect,creativeEffect:{
                prev:{
                  shadow:!0,translate:["-120%",0,-500]}
                ,next:{
                  shadow:!0,translate:["120%",0,-500]}
              }
              ,autoHeight:isNaN(t.autoHeight),watchOverflow:isNaN(t.watchOverflow),centeredSlides:isNaN(t.centeredSlides),autoplay:!!t.autoplay,watchSlidesProgress:!0,disableOnInteraction:t.disableOnInteraction,loop:isNaN(t.loop),freeMode:!!t.freeMode,minimumVelocity:t.minimumVelocity,momentum:!!t.momentum,keyboard:!!t.keyboard,mousewheel:!!t.mousewheel,navigation:{
                nextEl:"#".concat(o," .swiper-button-next"),prevEl:"#".concat(o," .swiper-button-prev")}
              ,breakpointsInverse:!0};
            function a(e){
              for(var n=[320,768,992,1200],r=n.findIndex((function(t){
                return t==e}
                                                         ));r<n.length;r++){
                var o=n[r];
                if(!isNaN(parseInt(t["ft-slides-".concat(o)],10)))return{
                  slidesPerView:parseInt(t["ft-slides-".concat(o)],10),spaceBetween:parseInt(t["ft-space-".concat(o)],10),slidesPerGroup:parseInt(t["ft-perGroup-".concat(o)],10)}
              }
              return{
                slidesPerView:parseInt(t.slidesPerView,10),spaceBetween:parseInt(t.spaceBetween,10),slidesPerGroup:parseInt(t.slidesPerGroup,10)}
            }
            var c={
              1200:a(1200),960:a(992),768:a(768),320:a(320)};
            c&&(i.breakpoints=c),["0","false","none"].includes(t.pagination)||(i.pagination={
              el:"#".concat(o," .swiper-pagination"),type:t.pagination,dynamicBullets:!!t.dynamicBullets,progressbarOpposite:!!t.progressbarOpposite,bulletElement:"div",clickable:!0}
                                                                              ),["cube","fade","flip"].includes(t.effect)&&(i.breakpointsInverse=!1,i.breakpoints={
            }
                                                                                                                           ),!0===t.autoplay?i.autoplay={
              delay:t.autoplayDelay,stopOnLastSlide:t.autoplayStopOnLastSlide,disableOnInteraction:t.autoplayDisableOnInteraction,reverseDirection:t.autoplayReverseDirection,waitForTransition:t.autoplayWaitForTransition}
            :i.autoplay=!1,t.scrollbar&&(i.scrollbar={
              el:"#".concat(o," .swiper-scrollbar"),draggable:!0}
                                        );
            var s="swiper-".concat(o);
            null==this||null===(e=this.classList)||void 0===e||e.add(s);
            var l=function(){
              var t="slider".concat(o);
              if(window[t])try{
                window[t].destroy(!0,!0)}
              catch(t){
                console.log("swipper slider",t)}
              window[t]=new Swiper(".".concat(s),i)};
            if(n&&"undefined"==typeof Swiper){
              var h=document.createElement("link");
              h.rel="stylesheet",h.href=r,document.body.appendChild(h);
              var u=document.createElement("script");
              u.src=n,u.onload=l,document.body.appendChild(u)}
            else l()}
           .bind(el))(props[el.id]);
        }
      </script>
</body>
</html>

