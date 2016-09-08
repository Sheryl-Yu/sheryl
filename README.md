<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, minimum-scale=1.0,
                                   maximum-scale=1.0">



      <title>Work with me &ndash; by Yu Zhan Qiong</title>

    <link rel="stylesheet"
          href="http://fonts.googleapis.com/css?family=Ubuntu:300,500,300italic">

    <style>


        /**
         * CSS is all inlined; there’s no point wasting an extra request for a
         * single-pager.
         */


        /**
         * Mediocre reset; do not use on sites of any reasonable size.
         */
        * {
            margin:  0;
            padding: 0;
            -webkit-box-sizing: border-box;
               -moz-box-sizing: border-box;
                    box-sizing: border-box;
        }

        /**
         * Single-direction margin declarations:
         * csswizardry.com/2012/06/single-direction-margin-declarations
         */
        h1, h2, h3, h4, h5, h6, hgroup,
        ul, ol, dl,
        blockquote, p, address,
        table, fieldset,
        figure, pre {
            margin-bottom: 24px;
            margin-bottom: 1.5rem;
        }

        ul, ol, dd {
            margin-left: 48px;
            margin-left: 3rem;
        }

        html {
            font: 300 100%/1.5 Ubuntu, sans-serif;
            background-color: #fff;
            color: #444;
        }

        /**
         * Set up the viewport to which our full-page bands will stick.
         */
        html,
        body {
            height: 100%;
        }

        a {
            color: #f43059;
            text-decoration: none;
        }

            a:hover {
                text-decoration: underline;
            }

        a, b, strong, dt {
            font-weight: 500;
        }

        h1, h2, h3, h4, h5, h6 {
            font-weight: 300;
            color: #f43059;
        }

        h1 {
            font-size: 36px;
            font-size: 2.25rem;
            line-height: 1.33333;
        }

        h2 {
            font-size: 30px;
            font-size: 1.875rem;
            line-height: 1.6;
        }

        h3 {
            font-size: 24px;
            font-size: 1.5rem;
            line-height: 1;
        }

        h4 {
            font-size: 20px;
            font-size: 1.25rem;
            line-height: 1.2;
        }

        h5 {
            font-size: 16px;
            font-size: 1rem;
            line-height: 1.5;
        }

        h6 {
            font-size: 14px;
            font-size: 0.875rem;
            line-height: 1.71429;
        }

        /**
         * 1. Force small text to honour its `line-height`.
         */
        small {
            font-size: 12px;
            font-size: 0.75rem;
            line-height: 2;
            display: inline-block; /* [1] */
            color: #999;
        }

        img {
            max-width: 100%;
            height: auto;
        }

        blockquote {
            text-indent: -0.394em;
        }

            blockquote p:before {
                content: "“";
            }

            blockquote p:after {
                content: "";
            }

            blockquote p:last-of-type:after {
                content: "”";
            }

            blockquote p:last-of-type {
                margin-bottom: 0;
            }

        .source {
            display: block;
            text-indent: 0;
        }

            .source:before {
                content: "—";
            }


        /**
         * Page constraint.
         *
         * 1. Clear floats. Using this method fixes a weird Firefox `max-width`
         *    issue on images. Bizarre.
         */
        .wrapper {
            width: 100%;
            max-width: 1200px;
            padding: 72px 24px 48px;
            margin-right: auto;
            margin-left:  auto;
            overflow: hidden; /* [1] */
        }


        /**
         * Full-width photo band.
         *
         * 1. Make the band stick to the top and bottom of the viewport.
         *
         * Photo credits:
         * Band 1: Ashley Baxter (@iamashley)
         * Band 2: Naomi Atkinson (@naomisusi)
         * Band 3: Stefan Nitzsche (@stn1978)
         * Band 4: Matti Besser (@m_besser)
         */
        .band {
            position: relative;
            min-height: 100%; /* [1] */
            background-color: #2a2a2a;
            background-position: center center;
            background-attachment: scroll;
            -webkit-background-size: cover;
               -moz-background-size: cover;
                    background-size: cover;
        }

        .band--01   { background-image: url(img/css/bands/01--small.jpg); }
        .band--02   { background-image: url(img/css/bands/02--small.jpg); }
        .band--03   { background-image: url(img/css/bands/03--small.jpg); }
        .band--04   { background-image: url(img/css/bands/04--small.jpg); }

        @media screen and (min-width: 480px) {

            .band--01   { background-image: url(img/css/bands/01--medium.jpg); }
            .band--02   { background-image: url(img/css/bands/02--medium.jpg); }
            .band--03   { background-image: url(img/css/bands/03--medium.jpg); }
            .band--04   { background-image: url(img/css/bands/04--medium.jpg); }

        }

        @media screen and (min-width: 720px) {

            .band--01   { background-image: url(img/css/bands/01--large.jpg); }
            .band--02   { background-image: url(img/css/bands/02--large.jpg); }
            .band--03   { background-image: url(img/css/bands/03--large.jpg); }
            .band--04   { background-image: url(img/css/bands/04--large.jpg); }

        }

        @media screen and (min-width: 1024px) {

            .band--01   { background-image: url(img/css/bands/01--huge.jpg); }
            .band--02   { background-image: url(img/css/bands/02--huge.jpg); }
            .band--03   { background-image: url(img/css/bands/03--huge.jpg); }
            .band--04   { background-image: url(img/css/bands/04--huge.jpg); }

        }


        /**
         * Fix the background on larger screens.
         */
        @media screen and (min-width: 1025px) {

            .band {
                background-attachment: fixed;
                box-shadow: 0 0 10px rgba(0, 0, 0, 0.25) inset;
            }

        }

            /**
             * Pointer arrow.
             */
            .band:before {
                content: "";
                position: absolute;
                bottom: 0;
                left: 50%;
                margin-left: -12px;
                z-index: 1;
                width:  24px;
                height: 24px;
                border: 0 solid #fff;
                border-width: 0 5px 5px 0;
                opacity: 0;
                -webkit-animation: arrow-fade 1.5s 0.5s 1 linear;
                   -moz-animation: arrow-fade 1.5s 0.5s 1 linear;
                        animation: arrow-fade 1.5s 0.5s 1 linear;
                -webkit-transform: rotate(45deg) translate3d(0, 0, 0);
                   -moz-transform: rotate(45deg) translate3d(0, 0, 0);
                        transform: rotate(45deg) translate3d(0, 0, 0);
            }

            @-webkit-keyframes arrow-fade {

                from {
                    bottom: 48px;
                    opacity: 0;
                }

                5% {
                    opacity: 1;
                }

                to {
                    bottom: 0;
                    opacity: 0;
                }

            }

            @-moz-keyframes arrow-fade {

                from {
                    bottom: 48px;
                    opacity: 0;
                }

                5% {
                    opacity: 1;
                }

                to {
                    bottom: 0;
                    opacity: 0;
                }

            }

            @keyframes arrow-fade {

                from {
                    bottom: 48px;
                    opacity: 0;
                }

                5% {
                    opacity: 1;
                }

                to {
                    bottom: 0;
                    opacity: 0;
                }

            }

            /**
             * Translucent overlay.
             */
            .band:after {
                content: "";
                position: absolute;
                top:    0;
                right:  0;
                bottom: 0;
                left:   0;
                background-color: rgba(0, 0, 0, 0.25);
            }


        /**
         * Optional floating tagline over bands.
         */
        .tagline {
            position: absolute;
            top: 50%;
            right: 24px;
            left:  24px;
            z-index: 1;
            font-size: 48px;
            font-size: 3rem;
            line-height: 1;
            text-align: center;
            color: #fff;
            text-shadow: 1px 1px 0 #000;
        }

        /**
         * Keep the tagline vertically centred at all sizes. It uses magic
         * numbers, I’m afraid :(
         *
         * 1. When on one line, this is half the band’s height.
         * 2. When on three lines, this is half the band’s height.
         * 3. When on two lines, this is half the band’s height.
         */
        .tagline {
            margin-top: -24px; /* [1] */
        }

        @media screen and (max-width: 422px) {

            .tagline {
                margin-top: -72px; /* [2] */
            }

        }

        @media screen and (min-width: 422px) and (max-width: 709px) {

            .tagline {
                margin-top: -48px; /* [3] */
            }

        }


        /**
         * Tabs.
         */
        .tabs {
            list-style: none;
            margin: 0;
            width: 100%;
            display: table;
            table-layout: fixed;
            text-align: center;
            background-color: #f43059;
            font-size: 12px;
            font-size: 0.75rem;
            line-height: 2;
        }

            .tabs > li {
                display: table-cell;
                vertical-align: middle;
                border: 0 solid rgba(0, 0, 0, 0.1);
                border-width: 0 1px;
                border-right-color: rgba(255, 255, 255, 0.15);
            }

            .tabs > li:first-child {
                border-left-width: 0;
            }

            .tabs > li:last-child {
                border-right-width: 0;
            }

                .tabs > li > a {
                    color: #fff;
                    padding: 12px;
                    display: block;
                    font-weight: 300;
                }

                .tabs__current {
                    text-decoration: underline;
                    cursor: text;
                }


        /**
         * Hovering little logo.
         */
        .logo {
            position: absolute;
            top:  24px;
            left: 24px;
            z-index: 1;
        }

            .logo__img {
                display: block;
                border-radius: 4px;
            }


        /**
         * Page-level stuff.
         */

        @media screen and (min-width: 720px) {

            /**
             * Abstract layout into a quasi-grid-system.
             */
            .content {
                margin-left: -72px;
                overflow: hidden;
            }

                .content__item {
                    display: inline-block;
                    vertical-align: top;
                    padding-left: 72px;
                }

                .content__sub {
                    width: 35%;
                }

                .content__main {
                    width: 65%;
                }

            /**
             * Reversed-order content blocks.
             */
            .content--rev {
                direction: rtl;
                text-align: left;
            }

                .content--rev .content__item {
                    direction: ltr;
                    text-align: left;
                }

        }

        .footer {
            font: 75%/1.5 sans-serif;
            background-color: #2a2a2a;
            color: #aaa;
            text-align: center;
        }

        @media screen and (min-width: 720px) {

            .footer {
                text-align: left;
            }

        }

            .footer a {
                color: #fff;
            }


        /**
         * Availability.
         */
        .availability {
            text-align: center;
            padding: 12px 24px;
            color: #fff;
        }

        .availability--available {
            background-color: #3f990f;
        }

        .availability--unavailable {
            background-color: #9f102e;
        }


        /**
         * Rhetorical intro.
         */
        .rhetorical {
            font-size: 20px;
            font-size: 1.25rem;
            line-height: 1.2;
        }

            .rhetorical > dt,
            .rhetorical > dd {
                display: inline;
            }

            .rhetorical > dd {
                margin-left: 0;
                color: #999;
            }


        /**
         * Client-list.
         */
        .client-list {
            list-style: none;
            margin-left: 0;
            overflow: hidden;
            text-align: center;
        }

            .client-list__item {
                padding: 12px;
                border: 0 solid #f0f0f0;
                border-top-width: 1px;
            }

            .client-list__item:first-child {
                border-top-color: transparent;
            }

            @media screen and (min-width: 720px) {

                /**
                 * Two-column layout on large enough devices.
                 */
                .client-list__item {
                    display: inline-block;
                    vertical-align: middle;
                    width: 50%;
                    padding: 24px;
                    border-width: 1px 0 0 1px;
                }

                /**
                 * Remove the borders from the first two (-n+2) items.
                 */
                .client-list__item:nth-of-type(-n+2) {
                    border-top-color: transparent;
                }

                /**
                 * Remove the borders from the first item in each pair (2n+1).
                 */
                .client-list__item:nth-of-type(2n+1) {
                    border-left-color: transparent;
                }

                /**
                 * Full-width items if it is the first in a theoretical pair,
                 * but the second in said pair is not present. Courtesy of
                 * Heydon Pickering: heydonworks.com/article/tetris-the-power-of-css
                 */
                .client-list__item:nth-of-type(2n+1):last-child {
                    width: 100%;
                }

            }

                /**
                 * 1. Logos are actually mask images, and their colours are set
                 *    via CSS.
                 * 2. Make all logos much paler when we hover the list of logos.
                 * 3. Make the single, currently hovered logo much darker.
                 */
                .client-list__logo {
                    display: block;
                    margin: 0 auto;
                    height: 47px;
                    background-color: #e4e4e4; /* [1] */
                    -webkit-transition: 0.5s;
                       -moz-transition: 0.5s;
                            transition: 0.5s;
                }

                .client-list:hover .client-list__logo {
                    background-color: #f5f5f5; /* [2] */
                }

                .client-list__item:hover .client-list__logo {
                    background-color: #ccc; /* [3] */
                }


        /**
         * Buttons. Lifted partly from beautons: github.com/csswizardry/beautons
         */
        .btn {
            display: inline-block;
            vertical-align: middle;
            white-space: nowrap;
            font-weight: 300;
            line-height: 3;
            padding-right: 24px;
            padding-left:  24px;
            background-color: #f43059;
        }

        .btn,
            .btn:hover,
            .btn:active,
            .btn:focus,
            .btn:visited {
                text-decoration: none;
                color: #fff;
            }

            .btn:active,
            .btn:focus {
                outline: none;
                position: relative;
                top: 1px;
            }

        .btn--full{
            width: 100%;
            padding-right: 0;
            padding-left:  0;
            text-align: center;
        }

        .btn--large {
            line-height: 6;
        }


        /**
         * Rules.
         */
        .rule {
            border: none;
            height: 1px;
            margin-bottom: 23px;
            background: #f0f0f0;
        }

        @media screen and (min-width: 720px) {

            .rule--mobile {
                display: none;
            }

        }

        @media screen and (max-width: 720px) {

            .rule--desktop {
                display: none;
            }

        }


        /**
         * Pull quotes.
         */
        .pull-quote {
            font-size: 18px;
            font-size: 1.125rem;
            line-height: 1.333333333;
            font-style: italic;
            color: #999;
            padding-left: 36px;
            border-left: 12px solid #f0f0f0;
        }

            .pull-quote__source {
                font-style: normal;
            }


        /**
         * quote-header.
         */
        .quote-header {
            font-family: sans-serif;
            font-weight: bold;
            font-size: 12px;
            font-size: 0.75rem;
            line-height: 2;
            text-align: right;
            margin-bottom: 0;
            color: #999;
        }


        /**
         * Price.
         */
        .price {
            text-align: center;
            color: #999;
        }

            .price__number {
                color: #666;
                display: inline-block;
                font-size: 64px;
                font-size: 4rem;
                line-height: 1.125;
            }


        /**
         * Yellow-fade.
         */
        .pull-quote:target {
            outline: 10px solid transparent;
            -webkit-animation: yellow-fade 5s;
               -moz-animation: yellow-fade 5s;
                    animation: yellow-fade 5s;
        }

        @-webkit-keyframes yellow-fade{
            5%{
                background-color:#ffc;
                outline: 10px solid #ffc;
            }
        }

        @-moz-keyframes yellow-fade{
            5%{
                background-color:#ffc;
                outline: 10px solid #ffc;
            }
        }

        @keyframes yellow-fade{
            5%{
                background-color:#ffc;
                outline: 10px solid #ffc;
            }
        }


        /**
         * Misc.
         */
        ::selection         { background-color: #f43059; color: #fff; }
        ::-moz-selection    { background-color: #f43059; color: #fff; }

    </style>

    <link rel="shortcut icon" href="http://csswizardry.com/icon.png">
    <link rel="apple-touch-icon-precomposed" href="http://csswizardry.com/icon.png">
    <meta name="apple-mobile-web-app-title" content="csswizardry">
    <meta name="description" content="Consultant Front-end Architect. CSS
    architecture and front-end performance expert available for work on
    interesting projects with nice people.">
</head>
<body>





    <div class="band  band--01" id="section-consultancy">

        <a href="#" title="Return to CSS Wizardry homepage" class="logo">
            <img src="img/brands/untitled.png" alt="CSS Wizardry" class="logo__img" width="64" height="64">
        </a>

        <h1 class="tagline">User Interface Designer</h1>

    </div><!-- /band -->





    <ul class="tabs">
        <li><a href="#section-consultancy" class="js-scroll  tabs__current">About me</a></li>
        <li><a href="#section-code-reviews" class="js-scroll">Work experience</a></li>
        <li><a href="#section-speaking" class="js-scroll">Wwards</a></li>
    </ul>





    <div class="wrapper">

        <section class="content">

            <div class="content__item  content__sub">

                <blockquote class="pull-quote" id="quote:andrew-clarke">
                    <p>So cool ! </p>
                    <b class="source  pull-quote__source"><a href="http://unfinished.bz/29">Sheryl Yu</a></b>
                </blockquote>

                <hr class="rule">

                <p class="availability  availability--available">
                My <strong>design work</strong> began in 2010.
                </p>

                <hr class="rule  rule--mobile">

            </div><!-- /content__sub





         --><div class="content__item  content__main">

                <h2>I work with tech teams to build great products…</h2>

                <dl class="rhetorical">

                    <dt>Want me to come and work in your office for a week?</dt>
                    <dd>Sounds like fun!</dd>

                    <dt>Starting an unusually large project?</dt>
                    <dd>Let me help you get started!</dd>

                    <dt>Want me to come and run a workshop for your team?</dt>
                    <dd>I’ll bring the doughnuts!</dd>

                </dl>

                <p>Hi~My name is Sherly Yu.
                I'm good at the human-computer interaction software, logic operation and the overall design of the beautiful interface.
                With a strong focus on performance, <b>pragmatism</b>, <b>agile</b>, and <b>strong development</b>, I like design, sustainable development.
                To know more <a href="/about/">About me</a>, or take a look at <a href="/csscv/">my work</a>.</p>

                <blockquote class="pull-quote" id="quote:andrew-betts">
                    <p>So cool ! <a href="https://www.xycool.com/">Test</a>,
                    web app.</p>
                    <b class="source  pull-quote__source"><a href="https://twitter.com/triblondon">Andrew Betts</a>,
                    Director, FT Labs</b>
                </blockquote>

                <p>All the fun things will probably be my job.</p>

                <ul class="client-list" id="section:clients">

                    <li class="client-list__item">
                        <img src="img/brands/sky.png" alt="BSkyB" class="client-list__logo" width="" height="47" />
                    </li><!--

                 --><li class="client-list__item">
                        <img src="img/brands/smashing-magazine.png" alt="Smashing Magazine" class="client-list__logo" height="47" />
                    </li><!--

                 --><li class="client-list__item">
                        <img src="img/brands/travelodge.png" alt="Travelodge" class="client-list__logo" height="47" />
                    </li><!--

                 --><li class="client-list__item">
                        <img src="img/brands/rizla.png" alt="Rizla" class="client-list__logo" height="47" />
                    </li><!--

                    <li class="client-list__item">
                        <img src="img/brands/ft.png" alt="Financial Times" class="client-list__logo" height="47" />
                    </li>--><!--

                 --><li class="client-list__item">
                        <img src="img/brands/booking.com.png" alt="Booking.com" class="client-list__logo" height="47" />
                    </li>

                </ul>

                <p>
                    <a href="mailto:harry@csswizardry.com?subject=Let%E2%80%99s%20work%20together"
                    class="btn  btn--full  btn--large">Get in touch</a>
                </p>

                <!--
                <blockquote class="pull-quote" id="quote:dan-bentley">
                    <p>Those floats were never going to clear themselves.</p>
                    <b class="source  pull-quote__source">Dan Bentley, Lead JS
                    Developer, Numiko</b>
                </blockquote>
                -->

            </div><!-- /content__main -->

        </section><!-- /content -->

    </div><!-- /wrapper -->










    <div class="band  band--02" id="section-code-reviews">
        <h2 class="tagline">: - ) Two</h2>
    </div><!-- /band -->





    <ul class="tabs">
        <li><a href="#section-consultancy" class="js-scroll">About me</a></li>
        <li><a href="#section-code-reviews" class="js-scroll  tabs__current">Work experience</a></li>
        <li><a href="#section-speaking" class="js-scroll">Wwards</a></li>
    </ul>





    <div class="wrapper">

        <section class="content">

            <div class="content__item  content__main">

                <h2>Code reviews</h2>

                <p>Do not know what to write. I want to write again : - )
                Unsure if you’re headed in the right direction? Have a mature
                   project that you’re struggling to scale? Interested to know
                   how you and your team can improve your work? Just want to
                   become a better developer? A remote CSS code review could be
                   <em>exactly</em> what you need.</p>

                <blockquote class="pull-quote" id="quote:darius-contractor">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source">Darius Contractor,
                    <a href="http://www.photosugar.com/">PhotoSugar</a></b>
                </blockquote>

                <p>Do not know what to write. I want to write again : - )
                 <i>one</i>. Do not know what to write. 
                 <b>one</b>, <b>two</b>,
                   <b>three</b>, <b>four</b>, <em>lot</em> more.</p>

                <p>How it works:</p>

                <ol>
                    <li>Do not know what to write. <strong>I want to write again</strong> : - )</li>
                    <li>Do not know what to write. <strong>I want to write again</strong> : - )</li>
                    <li>Do not know what to write. <strong>I want to write again</strong> : - )</li>
                </ol>

                <p>Do not know what to write.<a href="http://csswizardry.com/2013/11/code-reviews-as-a-service/">I want to write again</a>
                  : - )<em> : - )</em>  If you.
                  <a href="mailto:harry@csswizardry.com">email me</a>.</p>

                <p>Do not know what to write. I want to write again : - )</p>

            </div><!-- /content__main





         --><div class="content__item  content__sub">

                <blockquote class="pull-quote" id="quote:rob-farnell-01">
                    <p>More people need to benefit from what he has to offer.</p>
                    <b class="source  pull-quote__source">Lead Creative Designer</b>
                </blockquote>

                <hr class="rule">

                <p class="price">
                    <b class="price__number">999</b>^-^
                </p>

                <p>
                    <a href="mailto:harry@csswizardry.com?subject=Code%20review"
                    class="btn  btn--full  btn--large">Arrange a review</a>
                </p>

                <hr class="rule">

                <p><small>Terms and conditions apply.</small></p>

            </div><!-- /content__sub -->

        </section><!-- /content -->

    </div><!-- /wrapper -->










    <div class="band  band--03" id="section-speaking">
        <h2 class="tagline">: - ) Three</h2>
    </div><!-- /band -->





    <ul class="tabs">
        <li><a href="#section-consultancy" class="js-scroll">About me</a></li>
        <li><a href="#section-code-reviews" class="js-scroll">Work experience</a></li>
        <li><a href="#section-speaking" class="js-scroll  tabs__current">Wwards</a></li>
    </ul>





    <div class="wrapper">

        <section class="content  content--rev">
            
            <div class="content__item  content__main">

                <h2>Speaking and workshops</h2>

                <p>Do not know what to write. I want to write again : - )</p>

                <blockquote class="pull-quote" id="quote:roel-n">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source"><a href="https://twitter.com/pixelambacht/status/388665752234262528">Roel N</a></b>
                </blockquote>

                <p>Do not know what to write. 
                <a href="/speaking/">I want to write again</a>: - )</p>

                <blockquote class="pull-quote" id="quote:kimb-jones-01">
                    <p>Do not know what to write. </p>
                    <b class="source  pull-quote__source"><a href="https://twitter.com/mkjones">one</a>,
                       two, <a href="http://makedo.in/">three</a></b>
                </blockquote>

            </div><!-- /content__main





            --><div class="content__item  content__sub">

                <blockquote class="pull-quote" id="quote:peter-van-grieken">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source"><a href="https://twitter.com/petervangrieken/status/388615139102294016">Sheryl Yu</a></b>
                </blockquote>

                <hr class="rule">

                <p>
                    <a href="mailto:harry@csswizardry.com?subject=Request%20to%20speak"
                    class="btn  btn--full  btn--large">Book me</a>
                </p>

            </div><!-- /content__sub -->

        </section><!-- /content -->

    </div><!-- /wrapper -->










    <div class="band  band--04" id="section:testimonials">
        <h2 class="tagline">: - ) Four</h2>
    </div><!-- /band -->





    <ul class="tabs">
        <li><a href="#section-consultancy" class="js-scroll">About me</a></li>
        <li><a href="#section-code-reviews" class="js-scroll">Work experience</a></li>
        <li><a href="#section-speaking" class="js-scroll">Wwards</a></li>
    </ul>





    <div class="wrapper">

        <section class="content  content--rev">
            
            <div class="content__item  content__main">

                <h2>Testimonials</h2>

                <p>I’ve been lucky enough to work with some really great people
                   over the years, and some of them have said some really nice
                   things about me:</p>

                <h3 class="quote-header">Private workshop/consultancy client</h3>
                <blockquote class="pull-quote" id="quote:markus-klug">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source">
                        <a href="https://twitter.com/opus131">Markus Klug</a>
                    </b>
                </blockquote>

                <hr class="rule" />

                <h3 class="quote-header">Consultancy client</h3>
                <blockquote class="pull-quote" id="quote:matt-saunders">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source"><a href="https://twitter.com/matt5409">Matt
                        Saunders</a>, Web Developer, <a href="http://www.zealmedia.co.uk/">Zeal Media</a></b>
                </blockquote>

                <hr class="rule" />

                <h3 class="quote-header">Colleague</h3>
                <blockquote class="pull-quote" id="quote:rob-farnell-02">
                    <p>Do not know what to write. I want to write again : - ) <em>extra bit</em> </p>
                    <b class="source  pull-quote__source">Rob Farnell, Lead
                        Creative Designer, BSkyB</b>
                </blockquote>

                <hr class="rule" />

                <h3 class="quote-header">Colleague</h3>
                <blockquote class="pull-quote" id="quote:dan-rathbone">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source"><a href="http://thetrilemma.wordpress.com/">Dan Rathbone</a>,
                       Lead Performance Engineer, BSkyB</b>
                </blockquote>

                <hr class="rule" />

                <h3 class="quote-header">Workshop attendee</h3>
                <blockquote class="pull-quote" id="quote:rob-matwiejczyk">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source"><a href="https://twitter.com/RobMatwiejczyk/">Rob Matwiejczyk</a></b>
                </blockquote>

                <hr class="rule" />

                <h3 class="quote-header">Events organiser</h3>
                <blockquote class="pull-quote" id="quote:kimb-jones-02">
                    <p>Do not know what to write. I want to write again : - )</p>
                    <b class="source  pull-quote__source"><a href="https://twitter.com/mkjones">Kimb Jones</a>,
                       Director, <a href="http://makedo.in/">Make-Do</a></b>
                </blockquote>

                <p>If you’d like to be able to say nice things about me,
                <a href="mailto:harry@csswizardry.com?subject=Let%E2%80%99s%20work%20together">let’s work together on some stuff</a>!</p>

            </div><!-- /content__main





            --><div class="content__item  content__sub">

                <p>
                    <a href="mailto:harry@csswizardry.com?subject=Request%20to%20speak"
                    class="btn  btn--full  btn--large">Hire me</a>
                </p>

            </div><!-- /content__sub -->

        </section><!-- /content -->

    </div><!-- /wrapper -->










    <div class="footer">
        <div class="wrapper">

            <p>&copy; Sheryl Yu 2016 &bull;
            <a href="http://qiong.zcool.com.cn">@琼哚</a></p>

        </div><!-- /wrapper -->
    </div><!-- /footer -->

    <script>
        (function(){if("querySelector" in document&&"addEventListener" in window&&Array.prototype.forEach){var a=function(i,g){var m=16;var l=window.pageYOffset;var k=i.offsetTop;var e=k-l;var j=e/(g/m);var d;var h=function(){window.scrollBy(0,j);d()};var f=function(){clearInterval(c);setTimeout(function(){window.scrollTo(0,k)},m)};if(j>=0){d=function(){var n=window.pageYOffset;if((n>=(k-j))||((window.innerHeight+n)>=document.body.offsetHeight)){f()}}}else{d=function(){var n=window.pageYOffset;if(n<=(k||0)){f()}}}var c=setInterval(h,m)};var b=document.querySelectorAll(".js-scroll");[].forEach.call(b,function(c){c.addEventListener("click",function(g){g.preventDefault();var d=c.getAttribute("href");var h=document.querySelector(d);var f=c.getAttribute("data-speed");if(h){a(h,f||200)}},false)})}})();

        var _gaq = _gaq || [];
        _gaq.push(['_setAccount', 'UA-1856861-4']);
        _gaq.push(['_trackPageview']);

        (function() {
            var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
            ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
            var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
        })();
    </script>

</body>
</html>
