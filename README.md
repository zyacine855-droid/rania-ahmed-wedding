
.envelope.open:before{
transform:rotateX(180deg);
}

.card{
position:absolute;
width:260px;
height:160px;
background:white;
left:20px;
bottom:20px;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
color:#000;
transition:1s;
z-index:2;
}

.envelope.open .card{
transform:translateY(-170px);
}

.card h3{
font-family:'Great Vibes';
font-size:2rem;
color:#d4af37;
}

/* COUNTDOWN */

.countdown{
display:flex;
gap:20px;
margin-top:30px;
flex-wrap:wrap;
justify-content:center;
}

.box{
border:1px solid #d4af37;
padding:20px;
width:110px;
}

.box span{
display:block;
font-size:2rem;
color:#d4af37;
}

/* LOCATION */

.location-btn{
text-decoration:none;
background:#d4af37;
padding:15px 25px;
border-radius:30px;
color:black;
font-weight:bold;
margin-top:20px;
display:inline-block;
}

/* ANIMATION */

.fade{
opacity:0;
transform:translateY(30px);
transition:1s;
}

.fade.show{
opacity:1;
transform:translateY(0);
}

</style>
</head>
<body>

<section class="section">

<h1>Rania & Ahmed</h1>

<h2 class="gold">18 July 2026</h2>

<p>Tap the envelope to open your invitation</p>

<div class="envelope-wrapper" onclick="openInvitation()">

<div class="envelope" id="envelope">

<div class="card">
<h3>Save The Date</h3>
<p>Rania & Ahmed</p>
<p>18 July 2026</p>
</div>

</div>

</div>

</section>

<section class="section hidden fade" id="invitation">

<h1>We Are Getting Married</h1>

<h2 class="gold">Rania & Ahmed</h2>

<p>
Would be delighted to have you
celebrate this special day with us
</p>

<div class="countdown">

<div class="box">
<span id="days">0</span>
Days
</div>

<div class="box">
<span id="hours">0</span>
Hours
</div>

<div class="box">
<span id="minutes">0</span>
Minutes
</div>

<div class="box">
<span id="seconds">0</span>
Seconds
</div>

</div>

</section
