# <!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RifTrip - اكتشف الريف</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;background:#f5f7f2;color:#24352c}
header{background:#174c3b;color:white;text-align:center;padding:35px 15px}
header h1{font-size:42px;margin:5px}
header p{font-size:19px}
nav{background:#fff;padding:14px;text-align:center;position:sticky;top:0}
button{padding:10px 15px;border:0;border-radius:8px;background:#d99b43;color:#fff;font-weight:bold;margin:3px;cursor:pointer}
nav a{color:#174c3b;text-decoration:none;margin:8px;font-weight:bold}
main{max-width:1000px;margin:auto;padding:20px}
h2{color:#176047}
.hero{background:linear-gradient(#0005,#0006),url('https://images.unsplash.com/photo-1500375592092-40eb2168fd21?w=1400') center/cover;color:white;text-align:center;padding:90px 15px;border-radius:15px}
.hero h2{color:white;font-size:32px}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:18px}
.card{background:white;border-radius:12px;overflow:hidden;box-shadow:0 3px 12px #0001}
.card img{width:100%;height:170px;object-fit:cover}
.card div{padding:15px}
section{margin:35px 0}
.contact{background:#174c3b;color:white;padding:25px;border-radius:14px;text-align:center}
.contact h2{color:white}
.contact a{display:inline-block;margin:7px;padding:12px 16px;border-radius:8px;background:#fff;color:#174c3b;text-decoration:none;font-weight:bold}
footer{text-align:center;padding:20px;color:#667}
</style>
</head>
<body>
<header>
<h1>RifTrip</h1>
<p id="tagline">اكتشف الريف… وعِش التجربة</p>
</header>
<nav>
<button onclick="setLang('ar')">العربية</button>
<button onclick="setLang('fr')">Français</button>
<button onclick="setLang('en')">English</button>
<br><br>
<a href="#places" id="nav1">الوجهات</a>
<a href="#experiences" id="nav2">التجارب</a>
<a href="#contact" id="nav3">اتصل بنا</a>
</nav>
<main>
<div class="hero">
<h2 id="heroTitle">مرحبا بكم في الريف المغربي</h2>
<p id="heroText">اكتشف الطبيعة والبحر والثقافة الريفية الأصيلة</p>
</div>

<section id="places">
<h2 id="placesTitle">اكتشف أجمل الوجهات</h2>
<div class="cards">
<div class="card">
<img src="https://images.unsplash.com/photo-1500375592092-40eb2168fd21?w=700">
<div><h3 id="p1">بحيرة مارشيكا</h3><p id="d1">استمتع بجمال البحيرة ومناظرها الساحرة.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?w=700">
<div><h3 id="p2">شاطئ أركمان</h3><p id="d2">شاطئ جميل للاسترخاء والاستمتاع بالبحر.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?w=700">
<div><h3 id="p3">جبل كوروكو</h3><p id="d3">اكتشف الغابات والإطلالات الطبيعية الرائعة.</p></div>
</div>
<div class="card">
<img src="https://images.unsplash.com/photo-1510414842594-a61c69b5ae57?w=700">
<div><h3 id="p4">رأس الماء</h3><p id="d4">اكتشف جمال الساحل والقرى البحرية.</p></div>
</div>
</div>
</section>

<section id="experiences">
<h2 id="expTitle">عِش تجارب لا تُنسى</h2>
<div class="cards">
<div class="card"><div><h3 id="e1">رحلات الطبيعة</h3><p id="e1d">جولات واكتشاف للمناظر الطبيعية في الريف.</p></div></div>
<div class="card"><div><h3 id="e2">الثقافة الريفية</h3><p id="e2d">تعرف على العادات والتقاليد والتراث المحلي.</p></div></div>
<div class="card"><div><h3 id="e3">المطبخ المحلي</h3><p id="e3d">تذوق الأطباق والنكهات التقليدية الأصيلة.</p></div></div>
</div>
</section>

<section class="contact" id="contact">
<h2 id="contactTitle">تواصل معنا واحجز تجربتك</h2>
<p id="contactText">نحن هنا لمساعدتك في اكتشاف الريف المغربي.</p>
<a href="https://wa.me/212609619225">WhatsApp</a>
<a href="tel:+212609619225" id="call">اتصل بنا</a>
<a href="mailto:Driouchintegratedservices@gmail.com">Email</a>
<p>+212 609 619 225</p>
<p>Driouchintegratedservices@gmail.com</p>
</section>
</main>
<footer>© RifTrip - Discover the Rif</footer>

<script>
const translations={
ar:{
tagline:"اكتشف الريف… وعِش التجربة",nav1:"الوجهات",nav2:"التجارب",nav3:"اتصل بنا",
heroTitle:"مرحبا بكم في الريف المغربي",heroText:"اكتشف الطبيعة والبحر والثقافة الريفية الأصيلة",
placesTitle:"اكتشف أجمل الوجهات",p1:"بحيرة مارشيكا",d1:"استمتع بجمال البحيرة ومناظرها الساحرة.",
p2:"شاطئ أركمان",d2:"شاطئ جميل للاسترخاء والاستمتاع بالبحر.",
p3:"جبل كوروكو",d3:"اكتشف الغابات والإطلالات الطبيعية الرائعة.",
p4:"رأس الماء",d4:"اكتشف جمال الساحل والقرى البحرية.",
expTitle:"عِش تجارب لا تُنسى",e1:"رحلات الطبيعة",e1d:"جولات واكتشاف للمناظر الطبيعية في الريف.",
e2:"الثقافة الريفية",e2d:"تعرف على العادات والتقاليد والتراث المحلي.",
e3:"المطبخ المحلي",e3d:"تذوق الأطباق والنكهات التقليدية الأصيلة.",
contactTitle:"تواصل معنا واحجز تجربتك",contactText:"نحن هنا لمساعدتك في اكتشاف الريف المغربي.",call:"اتصل بنا"
},
fr:{
tagline:"Découvrez le Rif… vivez l'expérience",nav1:"Destinations",nav2:"Expériences",nav3:"Contact",
heroTitle:"Bienvenue dans le Rif marocain",heroText:"Découvrez la nature, la mer et la culture authentique du Rif",
placesTitle:"Découvrez nos destinations",p1:"Lagune de Marchica",d1:"Profitez de la beauté de la lagune et de ses paysages.",
p2:"Plage d'Arekmane",d2:"Une belle plage pour se détendre au bord de la mer.",
p3:"Mont Gourougou",d3:"Découvrez les forêts et les magnifiques panoramas.",
p4:"Ras El Ma",d4:"Découvrez la beauté du littoral et des villages marins.",
expTitle:"Vivez des expériences inoubliables",e1:"Excursions nature",e1d:"Explorez les paysages naturels du Rif.",
e2:"Culture rifaine",e2d:"Découvrez les traditions et le patrimoine local.",
e3:"Cuisine locale",e3d:"Goûtez aux plats et saveurs traditionnels.",
contactTitle:"Contactez-nous et réservez",contactText:"Nous sommes là pour vous aider à découvrir le Rif marocain.",call:"Appelez-nous"
},
en:{
tagline:"Discover the Rif… live the experience",nav1:"Destinations",nav2:"Experiences",nav3:"Contact",
heroTitle:"Welcome to the Moroccan Rif",heroText:"Discover nature, the sea and authentic Rif culture",
placesTitle:"Discover beautiful destinations",p1:"Marchica Lagoon",d1:"Enjoy the beauty of the lagoon and its stunning views.",
p2:"Arekmane Beach",d2:"A beautiful beach to relax and enjoy the sea.",
p3:"Mount Gourougou",d3:"Explore forests and wonderful natural views.",
p4:"Ras El Ma",d4:"Discover the beauty of the coast and fishing villages.",
expTitle:"Enjoy unforgettable experiences",e1:"Nature trips",e1d:"Explore the natural landscapes of the Rif.",
e2:"Rif culture",e2d:"Discover local traditions and heritage.",
e3:"Local cuisine",e3d:"Taste authentic traditional dishes and flavors.",
contactTitle:"Contact us and book your experience",contactText:"We are here to help you discover the Moroccan Rif.",call:"Call us"
}
};
function setLang(lang){
const t=translations[lang];
for(const key in t){const el=document.getElementById(key);if(el)el.textContent=t[key];}
document.documentElement.lang=lang;
document.documentElement.dir=lang==="ar"?"rtl":"ltr";
}
</script>
</body>
</html>
Discover the Beauty. Experience the Rif.
