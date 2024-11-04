# act1

```
SceneSetup.act1();
```

(...300)

n: VÀ ĐÂY LÀ SỰ LO ÂU CỦA CON NGƯỜI ĐÓ

n: _BẠN_ LÀ SỰ LO ÂU

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Ô kìa! Chúng ta lại quay lại đây lần nữa à?

`hong({eyes:"0_neutral"})`

n: VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI CỦA BẠN KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: THỰC TẾ LÀ, CHƠI LẠI GAME NÀY ĐANG ĐẶT HỌ VÀO *NGUY HIỂM* NGAY BÂY GIỜ

n: MAU LÊN, CẢNH BÁO HỌ!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Con người! Nghe này, chúng ta đang gặp nguy hiểm! Người chơi...

[...sẽ lại tra tấn chúng ta một lần nữa!](#act1_replay_torture)

[...sẽ không tìm thấy một kết thúc khác!](#act1_replay_alternate)

[...sẽ có mâu thuẫn giữa phần kể chuyện và gameplay!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Họ sẽ khiến chúng ta cuộn tròn thành một quả bóng và khóc!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Họ sẽ khiến chúng ta tiêu diệt điện thoại vì khiến bạn có một cơn hoảng loạn!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Họ sẽ khiến chúng ta *KHÔNG* đấm người chủ trì bữa tiệc!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Họ sẽ khiến chúng ta đấm người Phản Diện - Đồng Cảm chủ trì bữa tiệc!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Thì ít ra chúng ta có thể sẽ không nhảy khỏi mái nhà lần nà--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: HỌ SẼ KHIẾN CHÚNG TA NHẢY KHỎI MÁI NHÀ.
{{/if}}

`bb({body:"fear"});`

b: TẤT CẢ NHỮNG THỨ ĐÁNG SỢ NÀY SẼ XẢY RA VỚI CHÚNG TA, VÀ CHÚNG TA SẼ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Đúng, câu chuyện trên *toàn thể* vẫn y hệt, nhưng mỗi chương có hai kết thúc có thể đạt tới, cộng thêm đống cây phân nhánh lựa chọn đối thoạ--

`bb({body:"fear"});`

b: Người chơi sẽ thất vọng, đóng cửa sổ này, xóa phần mềm của chúng ta, và chúng ta sẽ--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Mau thực gì cơ?

`bb({eyes:"normal"});`

b: Cốt chuyện là về việc bạn có thể *LỰA CHỌN* xây dựng một mối quan hệ hợp tác với nỗi sợ của bạn,

`bb({eyes:"normal_right"});`

b: Nhưng chơi lại trò chơi sẽ cho ra cùng câu chuyện, ngầm nói rằng *LỰA CHỌN* của bạn không có ý nghĩa gì,

`bb({eyes:"narrow_eyebrow"});`

b: Tạo nên một sự mâu thuẫn giữa thông điệp và cơ chế của trò chơi,

`bb({eyes:"fear"});`

b: Qua đó phá hủy cấu trúc của không gian tự sự này,

`bb({body:"fear"});`

b: Và chúng ta sẽ--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: CHẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Được rồi chúng ta lại nhập vai nào.

```
Game.clearText();
```

n4: (ĐỂ SỰ LO ÂU CỦA _BẠN_ VÂN VÂN MÂY MÂY TƯƠNG TỰ NHẤT VỚI NỖI SỢ CỦA BẠN VÂN VÂN BẠN BIẾT THỪA RỒI MÀ)
```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Ô hay, con sói của tôi quay lại rồi. Tuyeeeeeệt thật.

`hong({eyes:"0_neutral"})`

n: VIỆC CỦA BẠN LÀ BẢO VỆ CON NGƯỜI CỦA BẠN KHỎI *NGUY HIỂM*

`bb({eyes:"look", mouth:"small_lock"})`

n: THỰC RA, CÁI BÁNH KẸP ĐÓ ĐANG ĐẶT HỌ VÀO *NGUY HIỂM* NGAY BÂY GIỜ

n: MAU LÊN, CẢNH BÁO HỌ!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Con người! Nghe này, chúng ta đang gặp nguy hiểm! Mối nguy hiểm là...

`bb({body:"squeeze"})`

n4: (ĐỂ SỰ LO ÂU CỦA _BẠN_ RA NÀO! CHỌN NHỮNG ĐIỀU TƯƠNG TỰ NHẤT VỚI NỖI SỢ CỦA BẠN)

(#act1_normal_choice)

# act1_normal_choice

[Chúng ta lại đang ngồi ăn trưa một mình! Lần nữa!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Chúng ta đang không hề năng suất trong khi ăn!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Bánh mì trắng đó không tốt cho chúng ta!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Bạn không biết rằng sự cô đơn có liên quan đến tử vong sớm ngang với việc hút 15 điếu thuốc mỗi ngày sao?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Ờ, cảm ơn vì đã trích dẫn nguồn thông tin nhưng--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Nghĩa là nếu chúng ta không chơi với ai *ngay bây giờ* chúng ta sẽ-

`bb({body:"panic"})`

b: CHẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: BẠN ĐÃ SỬ DỤNG *NỖI SỢ KHÔNG ĐƯỢC YÊU THƯƠNG*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Lấy máy tính của bạn ra và làm việc ngay bây giờ đi!

`hong({eyes:"0_annoyed"})`

h: Ơ, tôi thà không để vụn bánh rơi vào bàn ph--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nếu chúng ta không đóng góp cho xã hội thì chúng ta là kẻ ăn bám xã hội!

b: Quần chúng xã hội sẽ đến gặp bác sĩ xã hội để xin thuốc tiêu diệt những ký sinh trùng trong xã hội, sau đó chúng ta sẽ--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: CHẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: BẠN ĐÃ SỬ DỤNG *NỖI SỢ TRỞ THÀNH NGƯỜI XẤU*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Những nghiên cứu đó đã được lặp lại ch--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Lúa mì chế biến sẽ làm tăng lượng đường trong máu của chúng ta nên họ sẽ phải cắt bỏ tất cả các chi của chúng ta và sau đó chúng ta sẽ-

`bb({body:"panic"})`

b: CHẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾẾT

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: BẠN ĐÃ SỬ DỤNG *NỖI SỢ BỊ TỔN THƯƠNG*

(#act1b)

# act1b

n: NÓ CỰC HIỆU QUẢ

`bb({mouth:"smile", eyes:"smile"});`

b: Thấy không, con người? Tôi là con sói trung thành bảo vệ bạn! 

`bb({body:"pride_talk"});`

b: Tin tưởng trực giác của mình đi! Cảm xúc của bạn luôn có căn cứ mà!

`bb({body:"pride"});`

n: ĐƯA THANH NĂNG LƯỢNG CỦA CON NGƯỜI XUỐNG KHÔNG

n: ĐỂ BẢO VỆ NHU CẦU VỀ THỂ CHẤT + XÃ HỘI + ĐẠO ĐỨC CỦA HỌ, BẠN CÓ THỂ SỬ DỤNG:

n: NỖI SỢ *BỊ TỔN THƯƠNG* #harm#

n: NỖI SỢ *KHÔNG ĐƯỢC YÊU THƯƠNG* #alone#

n: VÀ NỖI SỢ *TRỞ THÀNH NGƯỜI XẤU* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (GỢI Ý: HÃY CHƠI NHỮNG LỰA CHỌN ĐÁNH VÀO NỖI SỢ HÃI SÂU SẮC, ĐEN TỐI NHẤT CỦA BẠN!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: biết gì không có lẽ bây giờ là thời điểm để xem điện thoại của mình.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: BẢO VỆ CON NGƯỜI CỦA BẠN

n: KHỎI THẾ GIỚI. KHỎI NGƯỜI KHÁC. KHỎI CHÍNH HỌ.

n: CHÚC MAY MẮN

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: VÒNG 1: *ĐÁNH!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Ớ. Facebook nói là sẽ có một bữa tiệc diễn ra vào cuối tuần này.

`bb({eyes:"uncertain"});`

b: Chẳng phải gã lập dị đó tổ chức tiệc *mọi* tuần sao?

`bb({eyes:"uncertain_right"});`

b: Họ đang cố lấp đầy khoảng trống tâm hồn nào vậy? Chắc hẳn bên trong họ rối tung lắm!

`hong({eyes:"surprise"});`

h: Này, mình có thư mời nè?

`bb({eyes:"fear", mouth:"normal"});`

b: Vậy thì!

[Đồng ý đi, không thì chúng ta sẽ chết vì cô đơn đó!](#act1c_loner)

[Từ chối đi, chúng chứa đầy các loại thuốc độc hại đó!](#act1c_drugs)

[Lờ nó đi, chúng ta chỉ làm mọi bữa tiệc buồn hơn thôi.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Mười lăm điếu thuốc mỗi ngày, con người ạ! Mười lăm!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Khi đó sẽ chẳng có ai đến dự đám tang của chúng ta, họ sẽ vứt tro cốt của chúng ta xuống biển, chúng ta sẽ bị cá voi ăn thịt,
{{/if}}

{{if !_.fifteencigs}}
b: và chúng ta trở thành PHÂN CÁ VOI!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Đúng vậy chúng ta nên đến bữa tiệc đó!
{{/if}}

{{if _.parasite}}
b: Chỉ cần mang theo máy tính để chúng ta có thể làm việc, và không trở thành kẻ ăn bám của xã hội.
{{/if}}

{{if _.whitebread}}
b: Miễn là họ không phục vụ BÁNH MÌ TRẮNG
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: LẠY CHÚA. Nếu điều đó khiến bạn im lặng, được thôi.

h: Tôi sẽ đồng ý.

{{if _.whalepoop}}
b: Phân cá voi đó, con người! Phân cá voi!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: hoặc tệ hơn... BÁNH MÌ TRẮNG
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Chúng ta sẽ dùng quá liều ma túy đá và bánh mì trắng đến nỗi họ sẽ không thể nhét vừa cái xác béo ú của chúng ta vào lò hỏa táng!
{{/if}}

{{if !_.whitebread}}
b: Chúng ta sẽ dùng quá liều nhiều loại thuốc đến nỗi người làm dịch vụ tang lễ sẽ tự hỏi làm sao cơ thể chúng ta *đã* được ướp xác trước!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Hơn nữa, không tiệc tùng được, chúng ta cần phải làm việc, nếu không chúng ta sẽ là kẻ ăn bám xã hội khủng khiếp!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: LẠY CHÚA. Nếu điều đó khiến bạn im lặng, được thôi.

h: Tôi sẽ từ chối.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tất cả những gì chúng ta làm là ngồi khóc trong góc về việc sự cô đơn nguy hiểm bằng việc hút 15 điếu thuốc mỗi ngày.
{{/if}}

{{if _.parasite}}
b: Tất cả những gì chúng ta làm trong các bữa tiệc là lo lắng làm sao để có thể làm việc hiệu quả.
{{/if}}

{{if _.whitebread}}
b: Tất cả những gì chúng ta làm là lo lắng về việc lựa chọn thực phẩm không lành mạnh sẽ giết chết chúng ta.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: trời tôi thắc mắc tại sao.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Vì thế nếu chúng ta đi, chúng ta sẽ khiến họ cảm thấy tệ, nhưng nếu chúng ta từ chối lời mời của họ chúng ta cũng sẽ khiến họ cảm thấy tệ!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TẤT CẢ NHỮNG GÌ CHÚNG TA LÀM LÀ LÀM MỌI NGƯỜI CẢM THẤY TỒI TỆ, VÌ VẬY CHÚNG TA NÊN CẢM THẤY TỒI TỆ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: LẠY CHÚA. Nếu điều đó khiến bạn im lặng, được thôi.

h: Tôi sẽ lờ đi lời mời đó.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Dù sao. Facebook là quá nhiều. Tôi cần thứ gì đó trầm lắng hơn, ít gây lo âu hơn.

`hong({eyes:"neutral"});`

h: Có gì mới trên Twitter?

`bb({eyes:"look"});`

[Ôi không, nhìn bản tin khủng khiếp đó kìa!](#act1d_news)

[Ôi không, cái tweet đó có đang bí mật nói về *chúng ta*?](#act1d_subtweet)

[Ê kìa, một cái GIF mèo uống sữa](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Chúa ơi, cảm giác như thế giới đang bốc cháy, nhỉ?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Cảm giác như mọi thứ đang kết thúc, như thể mọi thứ đang chết dần và chúng ta sắp phải chịu số phận bi thảm và không còn gì chúng ta có thể làm được nữa.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Retweet bản tin đó đi!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Được rồi mình sẽ retweet nó làm ơn nhỏ giọng xuống!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Thôi kệ đi, xem Snapchat nào.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: Đây là một dòng tweet ẩn! Một dòng subtweet đầy ẩn ý, ​​thật là ẩn ý!

`hong({eyes:"annoyed"});`

h: Có lẽ không phải là vậy?

`bb({eyes:"narrow", mouth:"small"});`

b: nhưng nếu như họ đều đang nói xấu sau lưng chúng ta thì sao

h: Họ không hề--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: ĐẰNG TRƯỚC LƯNG CHÚNG TA

`hong({eyes:"sad", mouth:"sad"});`

h: Mình khô--

`bb({eyes:"narrow", mouth:"small"});`

b: nhưng *nếu như*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *nếu như*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: được RỒI, mình sẽ thử Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Hehe ừ nó đáng yêu thật, vừa retweet nó xong, mình--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: MÈO KHÔNG THỂ TIÊU HÓA SỮA VÀ CHÚNG TA LÀ NHỮNG NGƯỜI TỒI VÌ THÍCH NGƯỢC ĐÃI ĐỘNG VẬT

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: được RỒI, mình sẽ thử Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Ớ, ảnh chụp từ tối qua. Vậy là những bữa tiệc hàng tuần như thế *đó* nhỉ.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Ồ, nhìn quá đông đúc đối với sự lo âu của tôi.

h: Có lẽ tôi đã không nên đồng ý với lời mời đó?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Thay đổi phản hồi á? Như một tên khốn nạn á?!](#act1e_yes_dontchange)

[Thay đổi phản hồi đi! Nó quá đông đúc!](#act1e_yes_changetono)

{{if _.subtweet}}
[Ừ họ hoàn toàn đang subtweet chúng ta.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Khoan chúng ta đã retweet mà chưa kiểm chứng thông tin.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Bạn biết rằng, tư thế của bạn thực sự rất tệ không?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Họ đã trông chờ chúng ta đến và giờ chúng ta phản bội lòng tin của họ sao? Bạn muốn chết vì cô đơn không?

{{if _.fifteencigs}}
b: MƯỜI. LĂM. ĐIẾU. THUỐC.
{{/if}}

{{if _.whalepoop}}
b: PHÂN. CÁ. VOI.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Im đi im đi tôi sẽ giữ nguyên là đồng ý!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Bạn không biết về các vụ giẫm đạp đám đông sao?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Năm 2003 một hộp đêm ở Rhode Island đã xảy ra hỏa hoạn và sự hoảng loạn đã khiến mọi người chặn lối thoát hiểm khiến 100 người bị thiêu chết-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: BẠN CÓ MUỐN ĐIỀU ĐÓ XẢY RA VỚI CHÚNG TA KHÔNG-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: TỪ CHỐI ĐI TỪ CHỐI ĐI TỪ CHỐI ĐI TỪ CHỐI ĐI TỪ CHỐI ĐI TỪ CH-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Im đi im đi tôi sẽ chuyển sang từ chối nó! Chúa ơi!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Ừm... trông vui thật đấy.

h: Có lẽ tôi đã không nên từ chối với lời mời đó?

`bb({mouth:"normal", eyes:"normal"});`

[Thay đổi phản hồi á? Như một tên khốn nạn á?!](#act1e_no_dontchange)

[Thay đổi phản hồi đi! Đừng chết trong cô đơn!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Ừ họ hoàn toàn đang subtweet chúng ta.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Khoan chúng ta đã retweet mà chưa kiểm chứng thông tin.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Bạn biết rằng, tư thế của bạn thực sự rất tệ không?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Mọi người đều đang trông cậy vào chúng mình!

b: ...để chúng ta để họ yên và để họ có một bữa tiệc vui vẻ mà không có một tên khốn kinh tởm {{if _.whitebread}}ăn-bánh-mì-trắng{{/if}} như chúng mì--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Im đi im đi tôi sẽ giữ nguyên là từ chối nó!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Sự cô đơn kéo dài làm tăng mức cortisol cũng như nguy cơ mắc bệnh tim mạch và đột quỵ!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: MƯỜI. LĂM. ĐIẾU. THUỐC.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Im đi im đi tôi sẽ chuyển thành đồng ý! Chúa ơi!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tất cả các dòng tweet tệ nạn của chúng mình đã quay lại gây ra vấn đề!
```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Chúng ta sẽ bị nêu tên, bị tẩy chay và bị kéo lê bằng dây thừng trên lưng ngựa trên xa lộ thông tin!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Tại sao cậu lại như thế này?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chúng ta đang phát tán thông tin sai lệch! Chúng ta đang phá hủy niềm tin vào nền báo chí tự do!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chúng ta là lý do chủ nghĩa phát xít sẽ trỗi dậy từ đống đổ nát của nền dân chủ!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Tại sao cậu lại như thế này?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Bạn có muốn có một cái bánh quy xoắn làm xương sống không?! Đừng cúi gằm xuống màn hình nữa!

```
bb({body:"meta"});
```

b: Bao gồm cả bạn nữa đó.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Tại sao cậu lại như thế này?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Ừm... trông vui thật đấy.

h: Có lẽ tôi đã không nên lờ đi lời mời đó?

`bb({mouth:"normal", eyes:"normal"});`

[Tiếp tục lờ họ đi, chúng ta vẫn là kẻ phá đám thôi.](#act1e_ignore_continue)

[Thực ra, đồng ý đi.](#act1e_ignore_changetoyes)

[Thực ra, từ chối đi.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Cứ lờ họ đi thì hơi bất lịch sự, đúng không?

`bb({eyes:"normal_right"});`

b: Thì những người khác luôn phớt lờ *chúng ta*, vậy đó

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: vậy thì chúng ta cứ coi là hòa thôi.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Cậu đang... để tôi vui vẻ sao?

b: Thì, ý tôi là, sự cô đơn *có thể* giết chết chúng ta.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Quá đông đúc. Các đám đông rất nguy hiểm.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Gì cũng được. Thông báo mới từ Tinder.

`bb({eyes:"uncertain"})`

b: Từ từ, ứng dụng tình ái ngắn hạn đó á?

`hong({eyes:"annoyed"})`

h: Nó không phải là một ứng dụng tình ái ngắn hạn, nó chỉ là một cách để gặp người mớ--

`bb({eyes:"narrow"})`

b: Nó là một ứng dụng tình ái ngắn hạn.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Ồ, mình có một cặp nè! Họ trông dễ thương đó!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Làm ơn hãy đừng phá hủy nó đối với m--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: NGUY HIỂM NGUY HIỂM NGUY HIỂM NGUY HIỂM NGUY HIỂM NGUY HIỂM

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Chúng ta *đang bị lợi dụng* bởi người khác.](#act1f_used_by_others)

[Chúng ta chỉ *đang lợi dụng* người khác.](#act1f_using_others)

[NGƯỜI ĐƯỢC CẶP VỚI BẠN LÀ SÁT NHÂN HÀNG LOẠT](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Những cuộc tình ái ngắn hạn ngẫu nhiên có thể lấp đầy khoảng trống ở đó,

b: nhưng chúng không bao giờ lấp đầy được khoảng trống...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: ở *đây*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tóm lại là CHÚNG TA SẼ CHẾT TRONG CÔ ĐƠN

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Bạn nghĩ bộ phận sinh dục của người khác là Pokémon để chúng ta sưu tập sao?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (nhạc nền pokémon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Tôi muốn trở thành, kẻ ^dâm dúa^ nhất-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Như chưa từng có ai như vậy-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Đùi và ^mông^, cặp ngực khêu gợi-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ với ^chim^ và ^hòn dái^!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: PERVY-MON! GOTTA CA-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tóm lại chúng ta là những kẻ thích thao túng biến thái.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Họ sẽ nhốt bạn dưới giếng và ép bạn ăn bánh mì trắng để vỗ béo bạn rồi chúng có thể mặc da bạn như một bộ đồ!
{{/if}}

{{if _.parasite}}
b: Họ sẽ đánh bạn bằng đồng hồ pomodoro và nói "BẠN NÊN LÀM VIỆC HIỆU QUẢ HƠN ĐỒ ĂN BÁM"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Họ sẽ xé xác bạn thành từng mảnh giấy vụn đẫm máu, biến ruột bạn thành những dải ruy băng, và trộn máu của bạn vào bát đựng rượu!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Thế NÀY thì sao có thể là lời mời dự tiệc được?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: mình chán trò chơi này lắm rồi.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"sự cô đơn sẽ giết chết chúng ta"... {{/if}}
{{if _.parasite}}"chúng ta là kẻ ăn bám xã hội"... {{/if}}
{{if _.whitebread}}"đừng ăn cái đó, nó sẽ giết chúng ta"... {{/if}}
{{if _.subtweet}}"họ đang nói xấu sau lưng chúng ta"... {{/if}}
{{if _.badnews}}"thế giới đang bốc cháy"... {{/if}}
{{if _.hookuphole}}"chúng ta sẽ chết trong cô đơn"... {{/if}}
{{if _.serialkiller}}"họ là sát nhân hàng loạt"... {{/if}}
{{if _.catmilk}}"mèo không thể tiêu hóa sữa"... {{/if}}
{{if _.pokemon}}bài hát chế tệ nạn... {{/if}}

h: mình chỉ muốn sống cuộc sống của mình.

h: mình chỉ muốn được tự do khỏi tất cả... nỗi đau này.

`bb({eyes:"look_sad"});`

b: Này... con người...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Sẽ ổn thôi.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Là con sói trung thành bảo vệ bạn, 
As your loyal guard-wolf, tôi sẽ luôn để mắt tới nguy hiểm và cố gắng hết sức để giữ bạn được an toàn.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Tôi hứa.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ứng dụng cuối cùng. Instagram. Chúng ta có gì nào?

`hong({eyes:"sad"});`

h: Đó... là thêm các ảnh bữa tiệc.

`hong({mouth:"sad"});`

h: Mọi người nhìn hạnh phúc quá. Tự do khỏi phiền muộn. Tự do khỏi lo âu.

`hong({mouth:"anger"});`

h: Chúa ơi, tại sao mình không thể như họ? Tại sao mình không thể chỉ *bình thường?*

`bb({eyes:"normal_right"});`

b: Nói về tiệc tùng, lời mời cuối tuần ấy. Đây là quyết định CUỐI CÙNG của tôi:

`bb({eyes:"normal"});`

[Chúng ta nên đi.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Chúng ta không nên đi.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Chúng ta n--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^MẸ KIẾP^.*

`hong({body:"2_you"});`

h: BẠN.

(...500)

b: s

(...1500)

`bb({eyes:"wat_2"});`

b: sao?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Tôi sẽ đồng ý với bữa tiệc đó,

{{if _.act1g=="go"}}
h: KHÔNG phải vì bạn muốn tôi làm thế, mà là vì *tôi* muốn làm thế.
{{/if}}

{{if _.act1g=="dont"}}
h: CHÍNH VÌ bạn không muốn tôi làm thế.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Cậu KHÔNG kiểm soát được mình.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Bây giờ thứ lỗi cho tôi để tôi có thể ăn chiếc bánh kẹp ngon lành này yên sự.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH CHÚNG TA SẼ CHẾT](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH MỌI NGƯỜI GHÉT CHÚNG TA](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH CHÚNG TA LÀ NHỮNG NGƯỜI TỒI](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH CHÚNG TA SẼ CHẾT AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH MỌI NGƯỜI GHÉT CHÚNG TA AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH CHÚNG TA LÀ NHỮNG NGƯỜI TỒI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CHÚC MỪNG

(...500)

n: BẠN ĐÃ BẢO VỆ THÀNH CÔNG NHU CẦU VỀ THỂ CHẤT + XÃ HỘI + ĐẠO ĐỨC CỦA CON NGƯỜI

n: ĐÓ, NHÌN XEM HỌ BIẾT ƠN NHƯ VẬY!

(...500)

n: GIỜ KHI THANH NĂNG LƯỢNG CỦA CON NGƯỜI LÀ KHÔNG, BẠN CÓ THỂ TRỰC TIẾP KIỂM SOÁT HÀNH ĐỘNG CỦA HỌ

`bb({mouth:"smile", eyes:"normal"});`

n: CHỌN NƯỚC ĐI CUỐI CỦA BẠN

`bb({mouth:"small_lock", eyes:"fear"});`

n: *KẾT LIỄU HỌ ĐI*

[{CHIẾN ĐẤU: Trừng phạt chiếc điện thoại gây căng thẳng của bạn!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{BỎ CHẠY: Cuộn tròn thành một quả bóng và khóc!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Chiếc điện thoại của bạn đã khiến bạn có một cơn hoảng loạn!

`bb({eyes:"anger"})`

b: Zuckerberg và đồng bọn đang lợi dụng sức khỏe tinh thần của bạn để kiếm tiền từ các nhà đầu tư mạo hiểm!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Trừng phạt điện thoại của bạn! Phá hủy nó! Tiêu diệt nó!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: TIÊU DIỆT NÓ TIÊU DIỆT NÓ TIÊU DIỆT NÓ TIÊU DIỆT NÓ TIÊU DIỆT NÓ TIÊU DIỆT NÓ TIÊU DIỆT NÓ TIÊU DIỆT NÓ TIÊU DIỆT NÓ T--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Cả thế giới đầy rẫy nguy hiểm!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Hãy làm như con tatu! Cuộn tròn thành một quả bóng để tự vệ!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: CUỘN TRÒN VÀ KHÓC CUỘN TRÒN VÀ KHÓC CUỘN TRÒN VÀ KHÓC CUỘN TRÒN VÀ KHÓC CUỘN TRÒN VÀ KHÓC CU--

(#act1j)

# act1j

`SceneSetup.act1_outro()`
