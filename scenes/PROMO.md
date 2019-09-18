# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[EMPEZAR!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Antes de empezar, ¿comó te gustaria leer?

`publish("show_options_bottom")`

# intro-start-2

n3: Ahora, a iniciar esta historia...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ESTO ES UN HUMANO

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: Y ESTA ES LA ANSIEDAD DEL HUMANO

n: _TU_ERES SU ANSIEDAD 

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nop. no, nope, no te escucho, voy a ver mi telefono

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: TU TRABAJO ES PROTEJER A TU HUMANO DEL *PELIGRO*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Suspiro!, estas pasando tu vida por Twitter! de nuevo!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Si, me pregunto por que no solo me siento y escucho a mis sentimientos mas seguido

`hong({eyes:"neutral"});`

n: RAPIDO, ADVIERTELE DEL *PELIGRO!*
  
```
bb({eyes:"look"});
```

[Oh no, mira esa horrible noticia!](#act1d_news)

[Oh no, es ese tweet hablando secretamente de *nosotros?*](#act1d_subtweet)

[Hey, un GIF de un gato tomando leche](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh, si, se ve bonito, y--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: LOS GATOS NO PUEDEN DIGERIR LECHE Y SOMOS PERSONAS HORRIBLES POR DISFRUTAR ABUSO ANIMAL

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



