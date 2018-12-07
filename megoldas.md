# Sz�m�t�g�pes j�t�kok weblap feladat megold�sa Bootstrap-el

----

## Feladatok
----

-[ ] �res Bootstrap HTML lap l�trehoz�sa

-[ ] Carousel beilleszt�s 3 k�ppel

-[ ] Jumbotron beilleszt�se

-[ ] Card elemek beilleszt�se

-[ ] Aloldalak l�trehoz�sa

----

## �res Bootstrap HTML oldal l�trehoz�sa

Brackets-ben �j f�jl, majd bem�soljuk az oldalt l�trehoz� HTML k�dot:

```html
<!doctype html>
<html lang="en">
<head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

    <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="bootstrap.css">

    <title>Bootstrap</title>
</head>
<body>
    <!-- Ide j�nnek az oldal tartalmai -->
   

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
</body>
</html>

```

----

## Carousel l�trehoz�sa

Ez az elem k�peket tud periodikusan megjelen�teni, annyit amennyit akarunk.

```html
 <div id="carouselExampleSlidesOnly" class="carousel slide" data-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active m-auto">
                <img class="d-block m-auto" style="height: 200px;" src="../" alt="C64">
            </div>
            <div class="carousel-item">
                <img class="d-block m-auto" style="height: 200px;" src="../" alt="Spacewar">
            </div>
            <div class="carousel-item">
                <img class="d-block m-auto" style="height: 200px;" src="../pong.png" alt="Pong">
            </div>
        </div>
    </div>
```
----

### Ezek a k�pek ker�ljenek be

>c64.png

>spacewar.png

>pong.png

Az alt seg�t a k�p hely�nek beazonos�t�s�ban.

## Jumbotron l�trehoz�sa

---

A k�vetkez� k�d hozza l�tre a Jumbotron-t

```html
<div class="jumbotron bg-info">
        <h1 class="display-4 text-dark">H1 sz�veg</h1>
        <p class="lead text-secondary">P sz�veg</p>
        <hr class="my-4">
        <!--<p>Inform�ci�k</p>
        <a class="btn btn-primary btn-lg" href="#" role="button">Tov�bbiak</a>-->
    </div>

```
### Ezek a sz�vegek jelenjenek meg

>H1:A sz�m�t�g�pes j�t�kok t�rt�nete
>P:A pongt�l a game boy-ig.


## Ismertet� sz�veg elhelyez�se

```html
<div class="container-fluid">
        <div class="row">
            <p class="text-justify m-2 p-2">
               Sz�veg ide
            </p>
        </div>
</div>
```

### Ez legyen a megjelen�tett sz�veg

Sz�m�t�g�pes j�t�kok t�rt�nete
A sz�m�t�g�pes j�t�kok t�rt�nete a sz�m�t�g�pek�vel k�zel azonos id�re vezethet� vissza. Az els� programoz�k csak a maguk sz�rakoztat�s�ra vagy a sz�m�t�g�p k�pess�geinek demonstr�l�s�ra k�sz�tett�k sz�m�t�g�pes j�t�kprogramjaikat. K�s�bb jelent meg az �zlet lehet�s�ge, ami �n�ll� iparr� tette a sz�m�t�g�pes j�t�kgy�rt�st. A sz�m�t�g�pekben rejl� lehet�s�gek bemutat�s�ra k�sz�tett j�t�kprogramok mind a mai napig fontos sz�nterei a fejleszt�seknek. Gondoljunk csak a sakkoz�g�pre. A Deep Blue az IBM �ltal kifejlesztett sz�m�t�g�p, amely sakkj�t�kban 1997-ben egy szab�lyszer� hatj�tszm�s p�ros m�rk�z�sen 3,5-2,5 ar�nyban legy�zte Garri Kaszparovot, az emberi sakkoz�s akkori vil�gbajnok�t. A c�l az volt, hogy bemutass�k, a sz�m�t�g�p nem �gy gondolkozik, ahogy az ember, de a nyers sz�m�t�si er� k�pes speci�lis esetekben az emberi gondolkod�ssal vetekedni.


## K�rty�k l�trehoz�sa, hivatkoz�ssal az aloldalakra

### El�sz�r egy kont�ner kell, amelyben a k�rty�kat egy sorba tessz�k bele

```html
 <div class="container">
        <div class="row">
		Ide j�nnek a k�rty�k
	</div>
</div>

```
## Egy k�rtya l�trehoz�sa

```html
 <div class="card h-100" style="width: 18rem;">
     <img class="card-img-top" src="../gameboy.png" alt="Card image cap">
              <div class="card-body">
                  <h5 class="card-title">Gameboy</h5>
                   <p class="card-text text-justify">A Game Boy az 	egyik els�, sikeres, nagy p�ld�nysz�mban eladott j�t�kkonzol. A jap�n Nintendo c�g �ltal tervezett �s gy�rtott 8-bites k�zi 	j�t�kkonzol egyik nagy el�nye a cser�lhet� j�t�kk�rtya volt.</p>
                    <a href="#" class="btn btn-primary">Tov�bb</a>
               </div>
</div>
```

