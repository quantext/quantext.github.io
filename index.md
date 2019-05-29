---
---
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="shortcut icon" type="image/x-icon" href="favicon.ico">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.6/css/bootstrap.min.css" integrity="sha384-rwoIResjU2yc3z8GV/NPeZWAv56rSmLldC3R/AZzGRnGxQQKnKkoFVhFQhNUwEyJ" crossorigin="anonymous">
    <link rel="stylesheet" href="/static/css/custom.css">
    <link rel="stylesheet" href="/static/css/index.css">

    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/brands.css" integrity="sha384-n9+6/aSqa9lBidZMRCQHTHKJscPq6NW4pCQBiMmHdUCvPN8ZOg2zJJTkC7WIezWv" crossorigin="anonymous">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/fontawesome.css" integrity="sha384-vd1e11sR28tEK9YANUtpIOdjGW14pS87bUBuOIoBILVWLFnS+MCX9T6MMf0VdPGq" crossorigin="anonymous">

    <link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700" rel="stylesheet">
    <link rel="stylesheet" href="/static/css/quantext-font/styles.css" />

    <script>
        var URL_FOR_SAVE_THEME = "/save_theme";
    </script>

    <title>Quantext</title>

    <!-- Global site tag (gtag.js) - Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=UA-108505400-1"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'UA-108505400-1');
    </script>
    
    <style>
    .main-theme-fill-dark:disabled {
        color: #aaa !important
    }

    .pretty.p-default.p-thick .state label:after, .pretty.p-default.p-thick .state label:before {
        margin-top: -.1rem
    }

    .p-setting.pretty .state label:before {
        color: #333 !important;
        border-color: #333 !important
    }

    .p-setting.pretty.p-default input:checked ~ .state label:after {
        background-color: #333 !important;
    }

    a {
        color: #57b0c2
    }
    </style>

</head>

<body>

    <div class="container-fluid" style="padding: 0 !important">
        <nav class="navbar navbar-toggleable-md">
            <nav class="navbar navbar-toggleable-md p-0 w-100">
                <button class="navbar-toggler p-0" style="margin-bottom:-10px" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="medium-quantext quantext-hamburger" style="cursor: pointer;"></span>
                </button>

                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav ml-auto centerFlex" style="width: 100%;">
                        <li class="nav-item"><a class="nav-link" href="/index" style="padding-left: 0;">Home</a></li>
                        <li class="nav-item"><a class="nav-link" href="/about">About</a></li>
                        <li class="nav-item" style="display:none"><a class="nav-link" href="/help">Help</a></li>
                        <li class="nav-item"><a class="nav-link" href="/research">Research</a></li>
                        <li class="nav-item" style="display:none"><a class="nav-link" href="/beta" style="color:crimson;text-transform: uppercase">Beta signup</a></li>
                        <div style="display:none">

                            <li class="btn btn-quantext login-nav">
                                <a class="" href="/login" style="font-size: .9rem;font-weight: 400;color: white;">Log in</a>
                            </li>
                            <li class="btn btn-quantext dark signup-nav">
                                <a class="" href="/login#signup" style="font-size: .9rem;font-weight: 400;color: white;">Sign up</a>
                            </li>

                        </div>
                    </ul>
                </div>
            </nav>
        </nav>
        <div style="position:relative;width:100%;height:500px;background:url('/static/img/quantext_feather_background.jpg');background-size: cover;background-position: top;">
            <div class="centerFlex p-4 main_duck">
                <img src="/static/img/quantext_title_white.svg" style="height: 60px;max-width:100%;"><div class="quantext-chunky-duck" style="color: white;font-size: 3rem;margin-bottom:-.5rem;margin-left: .5rem;"></div>
            </div>
            <div style="position:absolute;top:0;bottom:0;right:0;left:0;display:flex;align-items:center;flex-direction:column">
                <div id="big_index_title" style="margin-top:auto">Text analytics for higher education</div>
                <div id="big_index_subtitle" style="margin-bottom:auto">Analyse student writing in context</div>
            </div>
        </div>
        <div class="pt-4">
            {% for block in site.blocks %}
                {{ block.content | markdownify }}
            {% endfor %}            

            <div style="background:#111;padding:2rem 0">
                <div style="max-width:1200px;margin:0 auto;display:flex;flex-wrap:wrap" class="quantext_footer pl-3 pr-3">
                    <ul style="padding-left: 0;list-style: none;width:50%">
                        <li><a href="/index">Quantext home</a></li>
                        <li><a href="/about">About</a></li>
                        <li style="display:none"><a href="/help">Help</a></li>
                        <li><a href="/research">Research</a></li>
                    </ul>
                    <ul style="padding-left: 0;list-style: none;width:50%;display:none">
                        <li><a href="/beta">Beta signup</a></li>
                    </ul>
                    <div class="pt-4" style="width:100%;color:white">
                        Quantext<sup style="font-size:50%;top:-.5rem">TM</sup> is a registered trademark
                    </div>
                    <div class="pt-4" style="width:100%;color:white;font-size:2rem">
                        <a href="https://twitter.com/quantext" target="_blank"><i class="fab fa-twitter-square" style="color:white!important"></i></a>
                        <a href="https://github.com/quantext" target="_blank"><i class="fab fa-github-square" style="color:white!important"></i></a>
                    </div>
                </div>
            </div>
        </div>

    </div><!-- /.container-fluid -->

</body>

</html>
