# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Trước khi chúng ta bắt đầu, *bạn* muốn đọc như thế nào?

`publish("show_options_bottom")`

# intro-start-2

n3: Bây giờ, chúng ta cùng bắt đầu câu chuyện...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: ĐÂY LÀ MỘT CON NGƯỜI

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

n: VÀ ĐÂY LÀ SỰ LO ÂU CỦA CON NGƯỜI ĐÓ

n: _BẠN_ LÀ SỰ LO ÂU

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Không. Không, không, không nghe đâu. Mình sẽ xem điện thoại.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI CỦA BẠN KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Ôi! Bạn đang lướt hết cuộc đời của bạn trên Twitter! Lần nữa!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Ừ tôi tự hỏi tại sao mình không ngồi và lắng nghe suy nghĩ của mình thường xuyên hơn.

`hong({eyes:"neutral"});`

n: MAU LÊN, CẢNH BÁO HỌ VỀ MỘT MỐI *NGUY HIỂM!*

```
bb({eyes:"look"});
```

[Ôi không, nhìn bản tin khủng khiếp đó kìa!](#act1d_news)

[Ôi không, cái tweet đó có đang bí mật nói về *chúng ta*?](#act1d_subtweet)

[Ê kìa, một cái GIF mèo uống sữa](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Hehe ừ nó đáng yêu thật, mình--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG THỂ TIÊU HÓA SỮA VÀ CHÚNG TA LÀ NHỮNG NGƯỜI TỒI VÌ THÍCH NGƯỢC ĐÃI ĐỘNG VẬT

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



