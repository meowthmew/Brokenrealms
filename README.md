<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">


    <!-- ----------------------------------------------------------------- -->
    <!-- About Your Site                                                   -->
    <!-- ----------------------------------------------------------------- -->
    <link rel="shortcut icon" type="image/png" href="assets/favicon.png" />
    <title>Charadex</title>
    <meta property="title" content="Charadex" />
    <meta property="type" content="website" />
    <meta property="url" content="https://www.charadex.com/" />
    <meta property="image" content="assets/meta.png" />
    <meta name="description" content="A tool for organizing small ARPGs and species.">

    <!-- No AI scraping directives -->
    <meta name="robots" content="noai">
    <meta name="robots" content="noimageai">


    <!-- ----------------------------------------------------------------- -->
    <!-- Styles                                                            -->
    <!-- ----------------------------------------------------------------- -->

    <!-- Bootstrap CSS -->
    <!-- Using Bootstrap 4.5 because its closest to Toyhou.se's current version -->
    <!-- https://getbootstrap.com/docs/4.5/getting-started/introduction/ -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/css/bootstrap.min.css" integrity="sha384-TX8t27EcRE3e/ihU7zmQxVncDAy5uIKz4rEkgIXeMed4M0jlfIDPvg6uqKI2xXr2" crossorigin="anonymous">

    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />


    <!-- ----------------------------------------------------------------- -->
    <!-- Optional Styles                                                   -->
    <!-- ----------------------------------------------------------------- -->

    <!-- Custom CSS -->
    <link rel="stylesheet" type="text/css" href="styles/charadex.css">

    <!-- Google Font -->
    <link href="https://fonts.googleapis.com/css?family=Montserrat:400|Comfortaa:500" rel="stylesheet">


</head>

<body>


    <!-- --------------------------------------------------------------------
    <-- Header
    <-------------------------------------------------------------------- -->
    
    <div class="load-html" id="header" data-source="includes/header.html"></div>


    <!-- Spinner for loading-->
    <div class="spinner-border m-auto" id="loading"></div>


    <!-- --------------------------------------------------------------------
    <-- Terms
    <-- I've provided a boiler plate, edit these how you see fit!
    <-------------------------------------------------------------------- -->
    <div class="container softload py-md-5 my-4 py-4" id="main-container">
        <div class="row no-gutters m-n2">

            <!-- Main Content
            --------------------------------------------------------------------- -->
            <div class="col-12 p-2">
                <div class="card p-md-5 p-4 h-100">

                    <!-- Hero Image & Title
                    ------------------------------------------------------------- -->
                    <div class="hero-title mb-4" style="background-image: url();">
                        <div class="m-auto">Charadex</div>
                    </div>


                    <!-- Description
                    ------------------------------------------------------------- -->
                    <div class="px-4 text-muted">
                        <p>Write about your species...</p>
                    </div>


                    <!-- Links
                    ------------------------------------------------------------- -->
                    <hr class="my-4">
                    <div class="row no-gutters m-n1 mb-n2">

                        <div class="col-lg-4 p-1">
                            <h5>About</h5>
                            <div class="px-3">
                                <a class="btn btn-primary d-block mb-1" href="world.html">World</a>
                                <a class="btn btn-primary d-block mb-1" href="species.html">Species</a>
                                <a class="btn btn-primary d-block mb-1" href="masterlist.html">Designs</a>
                            </div>
                        </div>

                        <div class="col-lg-4 col-md-6 p-1">
                            <h5>Community</h5>
                            <div class="px-3">
                                <a class="btn btn-primary d-block mb-1" href="#">Toyhou.se</a>
                                <a class="btn btn-primary d-block mb-1" href="#">Discord</a>
                                <a class="btn btn-primary d-block mb-1" href="prompts.html">Prompts</a>
                            </div>
                        </div>

                        <div class="col-lg-4 col-md-6 p-1">
                            <h5>Resources</h5>
                            <div class="px-3">
                                <a class="btn btn-primary d-block mb-1" href="#">Help Desk</a>
                                <a class="btn btn-primary d-block mb-1" href="faq.html">FAQ</a>
                                <a class="btn btn-primary d-block mb-1" href="terms.html">TOS</a>
                            </div>
                        </div>

                    </div>


                    <!-- Social Media Links
                    ------------------------------------------------------------- -->
                    <hr class="mt-4">
                    <div class="text-center mb-md-n4 font-weight-bold">

                        <a class="mx-3" href="#"><i class="fas fa-floppy-disk fa-fw mr-1"></i> Toyhou.se</a>
                        <a class="mx-3" href="#"><i class="fab fa-discord fa-fw mr-1"></i> Discord</a>
                        <a class="mx-3" href="#"><i class="fab fa-twitter fa-fw mr-1"></i> Twitter </a>
                        <a class="mx-3" href="#"><i class="fab fa-tumblr fa-fw mr-1"></i> Tumblr</a>
                        <a class="mx-3" href="#"><i class="fas fa-cloud fa-fw mr-1"></i> BSky</a>

                    </div>
                </div>
            </div>


            <!-- Prompts
            --------------------------------------------------------------------- -->
            <div class="col-md-6 p-2" id="prompt-gallery">
                <div class="card p-md-5 p-4 h-100">

                    <h4 class="mb-0">Prompts</h4>
                    <hr class="mb-4">
                    <div class="list row no-gutters gallery-row m-n1"></div>

                    <div class="d-none">
                        <div class="col-12 gallery-item p-1" id="prompt-item">
                            <div class="card bg-faded p-3">
                                <h5 class="m-0">
                                    <a class="cardlink title" href=""></a>
                                </h5>
                                <hr class="my-2">
                                <div class="row no-gutters small my-n2">
                                    <div class="col-md-6 p-2 d-flex justify-content-between">
                                        <b>Starts</b> <span class="startdate"></span>
                                    </div>
                                    <div class="col-md-6 p-2 d-flex justify-content-between">
                                        <b>Ends</b> <span class="enddate"></span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>


            <!-- Staff
            --------------------------------------------------------------------- -->
            <div class="col-md-6 p-2" id="staff-gallery">
                <div class="card p-md-5 p-4 h-100">

                    <h4 class="mb-0">Staff</h4>
                    <hr class="mb-4">
                    <div class="list row no-gutters gallery-row m-n1"></div>

                    <div class="d-none">
                        <div class="col-md-6 gallery-item p-1" id="staff-item">
                            <div class="row no-gutters m-n1">
                                <div class="col-4 p-1 my-auto">
                                    <img class="img-fluid img-thumbnail image" src="">
                                </div>
                                <div class="col-8 p-1">
                                    <a class="d-block mt-2 link text-truncate" href=""><b class="username"></b></a>
                                    <span class="badge badge-primary jobtitle"></span>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>


            <!-- Designs
            --------------------------------------------------------------------- -->
            <div class="col-md-12 p-2" id="design-gallery">
                <div class="card p-md-5 p-4 h-100">

                    <h4 class="mb-0">Latest Designs</h4>
                    <hr class="mb-4">
                    <div class="list row no-gutters gallery-row m-n1"></div>

                    <div class="d-none">
                        <div class="col-md-3 col-6 gallery-item p-1" id="design-item">
                            <a class="card p-2 bg-faded d-block text-center cardlink" href="">
                                <img class="image img-fluid gallery-img" src=""><br>
                                <span class="btn btn-primary d-block mt-2 design"></span>
                            </a>
                        </div>
                    </div>

                </div>
            </div>



        </div>
    </div>


    <!-- --------------------------------------------------------------------
    <-- Footer
    <-------------------------------------------------------------------- -->
    
    <div class="load-html" id="footer" data-source="includes/footer.html"></div>


    <!-- ----------------------------------------------------------------- -->
    <!-- JS                                                                -->
    <!-- ----------------------------------------------------------------- -->

    <!-- JQuery -->
    <script src="https://code.jquery.com/jquery-3.6.0.js" integrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk=" crossorigin="anonymous"></script>

    <!-- Bootstrap -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ho+j7jyWK8fNQe+A12Hb8AhRq26LrZ/JpcUGGOn+Y7RsweNrtN/tE3MoK7ZeZDyx" crossorigin="anonymous"></script>

    <!-- List.js -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/2.3.0/list.min.js" crossorigin="anonymous"></script>

    <!-- Charadex Script -->
    <script src="styles/config.js"></script>
    <script src="styles/charadex.js"></script>
    <script>frontPage(options.index);</script>


</body>

</html>
