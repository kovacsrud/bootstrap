# Számítógépes játékok weblap feladat megoldása Bootstrap-el

----

## Feladatok
----

-[ ] Üres Bootstrap HTML lap létrehozása

-[ ] Carousel beillesztés 3 képpel

-[ ] Jumbotron beillesztése

-[ ] Card elemek beillesztése

-[ ] Aloldalak létrehozása

----

## Üres Bootstrap HTML oldal létrehozása

Brackets-ben új fájl, majd bemásoljuk az oldalt létrehozó HTML kódot:

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
    <!-- Ide jönnek az oldal tartalmai -->
   

    <!-- Optional JavaScript -->
    <!-- jQuery first, then Popper.js, then Bootstrap JS -->
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
</body>
</html>

```

----

## Carousel létrehozása

Ez az elem képeket tud periodikusan megjeleníteni, annyit amennyit akarunk.

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

### Ezek a képek kerüljenek be

>c64.png

>spacewar.png

>pong.png

Az alt segít a kép helyének beazonosításában.

## Jumbotron létrehozása

---

A következõ kód hozza létre a Jumbotron-t

```html
<div class="jumbotron bg-info">
        <h1 class="display-4 text-dark">H1 szöveg</h1>
        <p class="lead text-secondary">P szöveg</p>
        <hr class="my-4">
        <!--<p>Információk</p>
        <a class="btn btn-primary btn-lg" href="#" role="button">Továbbiak</a>-->
    </div>

```
### Ezek a szövegek jelenjenek meg

>H1:A számítógépes játékok története
>P:A pongtól a game boy-ig.


## Ismertetõ szöveg elhelyezése

```html
<div class="container-fluid">
        <div class="row">
            <p class="text-justify m-2 p-2">
               Szöveg ide
            </p>
        </div>
</div>
```

### Ez legyen a megjelenített szöveg

Számítógépes játékok története
A számítógépes játékok története a számítógépekével közel azonos idõre vezethetõ vissza. Az elsõ programozók csak a maguk szórakoztatására vagy a számítógép képességeinek demonstrálására készítették számítógépes játékprogramjaikat. Késõbb jelent meg az üzlet lehetõsége, ami önálló iparrá tette a számítógépes játékgyártást. A számítógépekben rejlõ lehetõségek bemutatására készített játékprogramok mind a mai napig fontos színterei a fejlesztéseknek. Gondoljunk csak a sakkozógépre. A Deep Blue az IBM által kifejlesztett számítógép, amely sakkjátékban 1997-ben egy szabályszerû hatjátszmás páros mérkõzésen 3,5-2,5 arányban legyõzte Garri Kaszparovot, az emberi sakkozás akkori világbajnokát. A cél az volt, hogy bemutassák, a számítógép nem úgy gondolkozik, ahogy az ember, de a nyers számítási erõ képes speciális esetekben az emberi gondolkodással vetekedni.


## Kártyák létrehozása, hivatkozással az aloldalakra

### Elõször egy konténer kell, amelyben a kártyákat egy sorba tesszük bele

```html
 <div class="container">
        <div class="row">
		Ide jönnek a kártyák
	</div>
</div>

```
## Egy kártya létrehozása

```html
 <div class="card h-100" style="width: 18rem;">
     <img class="card-img-top" src="../gameboy.png" alt="Card image cap">
              <div class="card-body">
                  <h5 class="card-title">Gameboy</h5>
                   <p class="card-text text-justify">A Game Boy az 	egyik elsõ, sikeres, nagy példányszámban eladott játékkonzol. A japán Nintendo cég által tervezett és gyártott 8-bites kézi 	játékkonzol egyik nagy elõnye a cserélhetõ játékkártya volt.</p>
                    <a href="#" class="btn btn-primary">Tovább</a>
               </div>
</div>
```

