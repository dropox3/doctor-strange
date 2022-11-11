# doctor-strange
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Leading Page Doutor Estranho</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous">
<link rel="stylesheet" href="style.css">
<link rel="stylesheet" href="animação.css">
<link rel="stylesheet" href="conteudo.css">
</head>
    <body>
    <section>
    </section>
    <section><section class="section-conteudo">
        <div class="container">
            <div class="row justify-content-center">
              <div class="col-12 col-md-6 mb-5">
                <div class="d-flex justify-content-center">
                    <div class="d-flex flex-column div-info">
                        <div class="p-2 div-titulo-principal">
                            <h1 class="titulo-principal">Deixe seu Email e Receba o Ingresso Exclusivo!</h1>
                        </div>
                        <div class="p-2">
                            <div class="input-group mb-3">
                                <input type="email" class="form-control input-cta" placeholder="seu@email.com" aria-label="Recipient's username" aria-describedby="basic-addon2">
                                <div class="input-group-append">
                                  <button class="btn btn-cta" type="button">Enviar</button>
                                </div>
                              </div>
                        </div>
                    </div>
                </div>
              </div>
              <div class="col-12 col-md-6 mb-5">
                <div class="d-flex justify-content-center">
                    <img class="img-fluid" src="img/ticket.png" alt="imagem ticket cinema">
                </div>
              </div>
            </div>
          </div>
    </section></section>
        <div class="div-secao-principal d-flex justify-content-between align-items-end">
            <div>
                <img class="img-clea aparece-e-foca-8s" src="img/clea.png" alt="Clea Doutor Estranho">
            </div>
            <div class="div-meio d-flex justify-content-center position-absolute">
               <div class="div-img-circulo  position-absolute">
                <img class="img-circulo rotacao "  src="img/circulo.png" alt="Circulo Girando">
               </div>
               <div class="div-img-drestranho position-absolute">
                <img class="img-drestranho aumenta-e-sobe" src="img/drestranho.png" alt="Doutor estranho">
               </div>
               <div class="div-img-titulo position-absolute"> 
                <img class="img-titulo"  src="img/titulo.png" alt="titulo">
               </div>
            </div>
            <div>
                <img class="img-wanda aparece-e-foca-4s d-none d-md-block" src="img/wanda.png" alt="Wanda">
            </div>
               </div>
    </section>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-OERcA2EqjJCMA+/3y+gxIOqMEjwtxJY7qPCqsdltbNJuaOe923+mo//f6V8Qbsw3" crossorigin="anonymous"></script>
</body>
</html>






style.css


body{
  background-color: black;
  color: white;
}



.div-secao-principal{
 background-image: url('../antigo/img/fundo.jpg') ;
 background-position: center;
 background-size: cover;
 min-height: 600px;

 color: white;
}

@media (max-width: 500px){
 .div-secao-principal{
  min-height: 600px;
 }

}





.img-clea{
  width: 100%;
  height: 600px;
  max-width: 900px;
  min-width: 540px;
  mix-blend-mode: lighten;
}

.img-wanda{
  width: 100%;
  height: 600px;
  min-width: 400px;
  mix-blend-mode: lighten;
}

.div-meio{
  height: 600px;
  width: 100%;
}

.img-circulo{
  width: 100%;
  max-height: 600px;
  mix-blend-mode: screen;
}

.img-drestranho{
    width: 100%;
    max-width: 700px;
}

.img-titulo{
 width: 100%;
 max-width: 500px;
 mix-blend-mode: screen;
 padding: 20px;
}

.div-img-circulo, .div-img-drestranho, .div-img-titulo{
  bottom: 0px;
}

conteudo.css

.section-conteudo{
    margin-top: 150px;
}

@media (max-width: 500px) {
    .section-conteudo{
        margin-top: 50px;
    }
}

.titulo-principal{
    font-family: 'Permanent Marker', cursive;
}

.div-info{
    max-width: 400px;
}

.btn-cta{
    background-color: #ffe509;
    min-height: 45px;
    color: #121418;
    border-radius: 0px 15px 15px 0px;

    font-weight: bold;
    font-size: 120%;
    font-family: 'Permanent Marker', cursive;
    padding: 10px;
    min-width: 120px;
}

.input-cta, .input-cta:focus{
    border: 2px solid #262626;
    min-height: 45px;
    border-radius: 15px 0px 0px 15px;
    background-color: transparent;
    color: white;
    }

.input-cta:focus{
    border-color: #ffe509;
    box-shadow: 0 0 0 0.25rem rgba(219, 205, 55, 0.09);
}


animação.css

.rotacao{
    animation: rotacao 8s ease-in-out infinite alternate;
}

@keyframes rotacao{
    0%{
            transform: rotate(0deg) translate(0px, 0px) scale(1);
    }
80%{
    transform: rotate(0deg) translate(0px, -70px) scale(1.05);
}
    100%{
             transform: rotate(360deg)  translate(0px, -70px) scale(1.3);
    }
}

.aumenta-e-sobe{
    animation: aumenta-e-sobe 4s ease infinite alternate;
}

@keyframes aumenta-e-sobe{
 0%{
    transform: scale(1) translate(0px, 0px);
 }
 90%{
    filter: brightness(1);
 }
 100%{
    transform: scale(1. 2) translate(0px, -44px);
    filter: brightness(1.3);
 }

}




.aparece-e-foca-4s{
    animation: aparece-e-foca 4s ease infinite alternate;
}

.aparece-e-foca-8s{
    animation: aparece-e-foca 6s ease infinite alternate;
}

@keyframes aparece-e-foca{
    0%{
        opacity: 0;
        filter: blur(10px);
    }
    80%{
        filter: blur(0px);
    }
    100%{
        opacity: 1;
        filter: blur(0px);
    }

}
