# intro

`SceneSetup.intro();`

# intro-play-button

[<div class="mini-icon" pic="play1"></div> BẮT ĐẦU! <div class="mini-icon" pic="play2"></div>](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: derp

`publish("show_options_bottom")`

# intro-start-2

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: ĐÂY LÀ MỘT CON NGƯỜI

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

`SceneSetup.act1();`

(...300)

n: VÀ ĐÂY LÀ SỰ LO ÂU CỦA CON NGƯỜI ĐÓ

n: _BẠN_ LÀ SỰ LO ÂU

[Chúng ta lại đang ngồi ăn trưa một mình! Lần nữa!](#act1a_alone) 

[Chúng ta đang không hề năng suất trong khi ăn!](#act1a_productive) 

[Bánh mì trắng đó không tốt cho chúng ta!](#act1a_bread)

# act1a_alone

`bb({mouth:"small", eyes:"narrow"})`

b: Bạn không biết rằng sự cô đơn có liên quan đến tử vong sớm ngang với việc hút 15 điếu thuốc mỗi ngày sao?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad et al, 2010, PLoS Medicine)

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ờ, cảm ơn vì đã trích dẫn nguồn thông tin nhưng--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Nghĩa là nếu chúng ta không chơi với ai *ngay bây giờ* chúng ta sẽ-

`bb({body:"panic"})`

b: CHẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("20p", "alone");
publish("hp_show");
```

(...2500)
