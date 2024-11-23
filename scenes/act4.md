# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (trò chơi đã tự động lưu)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *sigh*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Vậy thì bài học rút ra từ câu chuyện này là gì?

`hong({body:"one_up", eyes:"annoyed"})`

h: Chúng ta đã học được cái *quái* gì? Tôi *thực sự có* hành động ngu ngốc, "bạn bè" của tôi *thực sự có* lợi dụng tôi, và chúng ta suýt *chết*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Ừ, mà chưa tính cả hóa đơn viện phí á.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Ừ, mà chưa tính cả tổn thương gan á.](#act4a_liver)
{{/if}}

[Ừ, đó *là* tình huống xấu nhất á.](#act4a_worst)

[Ừ, tôi đã đúng.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Ừ. Mình không nghĩ là bảo hiểm của mình có chi trả cho việc "trở thành một kẻ ^ngốc tử^".

`hong({eyes:"annoyed", mouth:"normal"});`

b: Vậy mà... chúng ta đã sống sót!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Chúng ta chắc chắn đã mất đi vài năm tuổi thọ của mình...

`bb({eyes:"surprise"});`

b: Nhưng ít nhất chúng ta vẫn *có* tuổi thọ! Chúng ta đã sống sót!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Vậy mà...

h: Hm?

`bb({eyes:"surprise"});`

b: Chúng ta đã sống sót!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Nhưng... bạn cũng đúng.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Tôi *là* con sói đã giả vờ kêu sói. Vì vậy, khi nguy hiểm *thực sự* xảy ra, bạn – một cách chính đáng – đã không tin tôi.

`bb({eyes:"surprise_r"});`

b: Vậy mà, chúng ta đã sống sót!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Bất chấp mọi chuyện, chúng ta vẫn ở đây.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Bạn có vẻ khá bình tĩnh khi chúng ta vừa trải qua một trải nghiệm suýt chết.
{{/if}}

{{if !_.INJURED}}
h: Cậu có vẻ khá bình tĩnh khi chúng ta vừa trải qua một trải nghiệm *suýt* suýt chết.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Thì, nó làm cho mọi thứ khác bớt đáng sợ hơn khi so sánh. Nó cũng khiến tôi suy nghĩ.

`bb({eyes:"normal", mouth:"normal"});`

b: Nếu việc tôi đánh nhau với bạn là tệ, vì nó không bảo vệ được bạn...

h: Nhưng việc tôi đánh nhau với bạn *cũng* tệ, vì nó chỉ khiến bạn hét lớn hơn...

`bb({eyes:"normal_r"})`

b: Thì có lẽ...

`bb({eyes:"normal"})`

h: Có lẽ chúng ta không phải đánh nhau.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Tôi không phải là một con Sói hung dữ. Nhưng tôi cũng không phải là một chú chó canh gác.

`bb({eyes:"sad_d"})`

b: Tôi là một chú chó bị bỏ rơi ở trại cứu hộ.

`bb({eyes:"sad"})`

b: Chúng ta đã trải qua nhiều thứ khó khăn. Có lẽ là chấn thương hoặc bị bỏ bê. Đó là lý do tại sao đôi khi tôi phản ứng thái quá và nói:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Nhưng tôi không *muốn* trở thành một chú chó hèn nhát! Tôi muốn bảo vệ bạn! Tôi muốn trở thành một chú chó ngoan!

`bb({eyes:"sad", mouth:"normal"});`

b: Con người... bạn có thể giúp thuần hóa con sói này không?

`hong({eyes:"sad"})`

h: Tôi... Tôi sẽ cố.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Được rồi. Mối quan hệ lành mạnh với cảm xúc. Mối quan hệ cần giao tiếp. Vậy, hãy giao tiếp.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Năm phút tiếp theo sẽ nghe có vẻ rất sến súa, nhưng hãy giả vờ cho đến khi chúng ta làm được.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Con sói tâm hồn thân mến... *bạn* cảm thấy thế nào?

n2: TỔNG NHỮNG NỖI SỢ ĐÃ SỬ DỤNG:

n2: *BỊ TỔN THƯƠNG* {{_.attack_harm_total}}, *KHÔNG ĐƯỢC YÊU THƯƠNG* {{_.attack_alone_total}}, *TRỞ THÀNH NGƯỜI XẤU* {{_.attack_bad_total}}

n2: BẠN MUỐN NÓI VỀ NỖI SỢ NÀO ĐẦU TIÊN? (BẠN CÓ THỂ NÓI VỀ NHỮNG ĐIỀU KHÁC SAU)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Tôi sợ chúng ta sẽ bị tổn thương.](#act4_harm)

[Tôi sợ chúng ta sẽ cô đơn.](#act4_alone)

[Tôi sợ chúng ta là người xấu.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Tôi muốn bảo vệ nhu cầu an toàn về thể chất của bạn,

`bb({eyes:"sad_d"})`

b: Nhưng *toàn bộ thế giới* có vẻ rất nguy hiểm. Đầy rẫy bi kịch và cái ác.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Tôi không biết nữa, hơi đủ về việc *tôi* chọn điều gì để nói tiếp theo. *Bạn* sẽ nói gì, con người?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Một lần nữa, quay về bạn, con người. Bạn nghĩ sao?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Còn suy nghĩ gì nữa không, con người?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Bạn nói đúng. Hãy cùng tự vệ cho chúng ta.](#act4_harm_skills)

[Hãy tiếp xúc với *nhiều* nguy hiểm hơn.](#act4_harm_exposure)

[Cảm ơn bạn.](#act4_thanks) `_.thanks_for = "an toàn về mặt thể chất";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Nhưng... bằng cách nào? Tôi có nanh và móng vuốt, nhưng tôi chỉ là ẩn dụ thôi.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Chúng ta có thể học cách tự vệ? Tham gia một cộng đồng bảo vệ lẫn nhau? Cải thiện sức khỏe tổng quát và ranh giới cá nhân?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Có thể, nhưng...

[Chúng ta nên bắt đầu từ đâu?](#act4_harm_skills_start)

[Rủi chúng vẫn không hoạt động thì sao?](#act4_harm_skills_work)

[Rủi chúng ta quá chú trọng vào "an toàn" thì sao?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Có quá nhiều việc phải làm, quá nhiều thứ chúng ta cần phải sửa đổi về bản thân mình. Chúng ta thậm chí *bắt đầu* từ đâu?

`hong({ body:"shrug", eyes:"surprise" })`

h: Chúng ta đang bắt đầu ngay bây giờ.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ể?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Chúng ta đang thực hành giao tiếp tốt ngay bây giờ. Điều này sẽ giúp chúng mình phát hiện nguy hiểm tốt hơn, với ít cảnh báo sai hơn,

`hong({ eyes:"surprise" });`

h: Và *điều đó* sẽ giúp bảo vệ chúng ta khỏi nguy hiểm!

`hong({ eyes:"normal", mouth:"normal" });`

h: Do đó: đây *là* luyện tập cho việc tự vệ.

`bb({ eyes:"normal_r" })`

b: Ờ. Tôi vừa mong đợi nhiều hơn của cái này á:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Đúng là không có cách nào có thể bảo vệ chúng ta 100%...

`hong({ body:"one_up" });`

h: Nhưng ngay cả sự cải thiện chỉ 1% vẫn có giá trị, phải không?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Bạn thấy cái ly không phải rỗng 99%, mà là đầy 1%?

`bb({ eyes:"normal" });`

h: Vẫn có giá trị nếu bạn bị mắc kẹt trong sa mạc.

`bb({ eyes:"closed" });`

b: Được thôi. Nâng ly nào.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Ý tôi là, lý do duy nhất khiến bạn bỏ qua lời cảnh báo của tôi là vì *tôi* đã quá chú trọng vấn đề an toàn!

`bb({ body:"normal", eyes:"normal" })`

h: Không, bạn nói đúng. Chúng ta muốn thực hiện an toàn ở mức độ vừa phải. Mọi thứ đều ở mức độ vừa phải.

`bb({ eyes:"suspect" })`

b: Xin lỗi, *MỌI THỨ* đều ở mức độ vừa phải?

`hong({ eyes:"annoyed" })`

h: *Một lượng vừa phải các thứ* ở mức độ vừa phải.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Cảm ơn bạn đã đưa ra những tuyên bố nhất quán một cách đệ quy.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *CÁI GÌ*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Ý tôi là, giả sử một con chó sợ sấm sét.

`hong({ body:"hands_1" });`

h: Một mẹo mà người huấn luyện sử dụng là phát một bản ghi âm tiếng sấm ở mức âm lượng thấp, sau đó thưởng cho chó vì đã giữ được bình tĩnh.

`hong({ body:"hands_2" });`

h: Trong nhiều ngày, người huấn luyện sẽ tăng dần âm lượng cho đến khi chú chó vượt qua được nỗi sợ sấm sét.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Nó được gọi là liệu pháp tiếp xúc!

`hong({ body:"point", eyes:"normal" });`

h: Vì bạn là một chú chó, nên điều này cũng có tác dụng với bạn, đúng không? Tất cả các loài động vật có vú đều có phản ứng chiến đấu hoặc bỏ chạy giống nhau.

`hong({ body:"normal" });`

[Nếu chúng ta vô cảm *quá* thì sao?](#act4_harm_exposure_overboard)

[Nếu chúng ta tiếp xúc với nguy hiểm *thực sự* thì sao?](#act4_harm_exposure_hurt)

[Tôi là sói, không phải chó.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Và tôi sẽ cho bạn thấy lòng tốt và sự kiên nhẫn cho đến khi bạn được thuần hóa thành một chú cún con dễ thương.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Ỏ.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Chúng ta *vừa* thấy điều gì xảy ra nếu bạn dập tắt nỗi sợ hãi của mình – bạn tự đưa mình vào những tình huống *thực sự* nguy hiểm.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Hơn nữa, liệu việc mất cảm giác *quá* có biến chúng ta thành những kẻ tâm thần không?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Chẳng mấy chốc chúng ta sẽ tự thưởng cho mình khi xem phim khiêu dâm giết người bằng thuốc hít!

`hong({ eyes:"annoyed" })`

h: Mình... nghĩ rằng có một ranh giới giữa điều đó và tiếng sấm.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Nhưng chính xác *ở đâu*, con người? *Ở đâu?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Mình không biết. Nhưng *bạn* có thể giúp mình!

`hong({ eyes:"normal", body:"normal" })`

h: Làm việc và thương lượng với bạn, chúng ta sẽ tạo ranh giới đó.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Được. Nhưng tôi không có ngón tay cái nào đối diện, vì vậy bạn sẽ vẽ nó.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Thí dụ: chúng ta đã nhảy khỏi một cái *mái nhà*!
{{/if}}

{{if !_.INJURED}}
b: Thí dụ: chúng ta đã suýt nhảy khỏi một cái *mái nhà*!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Mà bạn nói đúng. Người ta *có thể* đi quá xa.

`hong({ eyes:"normal" });`

h: Nhưng đó là lý do tại sao, nếu chúng ta thực hiện liệu pháp tiếp xúc, chúng ta sẽ bắt đầu từ những bước nhỏ và tiến dần lên.

h: Ngay trước khi chúng ta gặp phải nguy hiểm *thực sự*, chúng ta dừng lại.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Vâng, tôi phân biệt được giữa việc nghe thấy tiếng sấm lớn, và việc đứng trong cơn bão với chiếc mũ nhọn cao.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Khoan đã, không có lý lẽ nào ủng hộ hay phản đối những gì tôi đang cảm thấy sao? Chỉ là... "cảm ơn" thôi sao?

`hong({ eyes:"surprise", body:"shrug" })`

h: Đúng vậy! Cảm ơn bạn đã quan tâm đến sự {{_.thanks_for}} của tôi.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Bạn ổn chứ?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Bạn chưa bao giờ nói *cảm ơn* với tôi trước đây.

`hong({ mouth:"smile" });`

h: Ôi, con sói hoảng loạn lông lá to đùng kia.

(#act4_something_else)

# act4_thanks_2

h: Ngay cả khi bạn phản ứng thái quá, tôi vẫn đánh giá cao việc bạn quan tâm đến sự {{_.thanks_for}} của tôi.

`bb({ eyes:"annoyed" })`

b: Đợi đã... bạn không chỉ lặp lại "cảm ơn" để tránh thực sự nói về những nỗi sợ này, phải không?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Vâng, mọi thứ phức tạp, và tôi không phải lúc nào cũng có sẵn câu trả lời.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Cuộc sống không đưa cho bạn danh sách gồm 3 câu trả lời đối thoại được tạo sẵn đâu.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Nhưng bây giờ, ít nhất tôi có thể nói lời cảm ơn.

b: Ừ, cảm ơn bạn, vì đã kiên nhẫn lắng nghe tôi.

`bb({ eyes:"closed" });`

b: Động vật có vú nhỏ nhắn không lông.

(#act4_something_else)

# act4_thanks_3

h: Kể cả khi tiếng sủa của anh làm tôi sợ, anh chỉ đang cố bảo vệ sự {{_.thanks_for}} của tôi thôi.

`bb({ eyes:"smile_r" });`

b: Được thôi, nếu anh cứ nịnh tôi thế này, internet sẽ có những ý tưởng kỳ lạ về chúng ta mất.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Thôi nào, tôi chỉ là một đứa trẻ tuổi đại học dễ bị tổn thương và anh là một con sói to lớn, đáng sợ. Điều tồi tệ nhất mà anh có thể--

`hong({ eyes:"normal", body:"point" });`

h: Thực ra, đừng trả lời câu hỏi đó.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Tôi muốn đảm bảo rằng bạn đáp ứng được nhu cầu sâu sắc của con người là được hòa nhập...

`bb({ eyes:"sad_u" });`

b: Nhưng tôi lo rằng nếu bất kỳ ai biết chúng ta – con người *thực* của chúng ta – thì chúng ta sẽ dọa họ bỏ chạy mất.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Tôi không biết nữa, hơi đủ về việc *tôi* chọn điều gì để nói tiếp theo. *Bạn* sẽ nói gì, con người?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Một lần nữa, quay về bạn, con người. Bạn nghĩ sao?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Còn suy nghĩ gì nữa không, con người?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Đồng ý: hãy cải thiện đời sống xã hội của chúng ta.](#act4_alone_skills)

[Mình nghĩ mọi người thích chúng ta. Thử nhé?](#act4_alone_experiment)

[Cảm ơn bạn.](#act4_thanks) `_.thanks_for = "thuộc về cộng đồng";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Chúng ta có thể rèn luyện các kỹ năng như đặt câu hỏi, lắng nghe và đồng cảm, cởi mở và dễ bị tổn thương, vân vân... không?

`hong({ eyes:"normal_l" });`

h: Hoặc tạo thói quen giao tiếp xã hội tốt hơn, như lên lịch thời gian với bạn bè hoặc thường xuyên đi gặp gỡ?

`hong({ body:"one_up" });`

h: Cũng có thể học cách thoải mái hơn khi bị từ chối.

`hong({ eyes:"normal" });`

h: Hoặc học cách biết khi nào mọi người *không* từ chối chúng ta, họ chỉ mệt mỏi hoặc có Khuôn mặt ^Thốn^ Nghỉ ngơi.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Có rất nhiều lựa chọn. Nhưng, về "học các kỹ năng xã hội"...

[Điều đó không phải là *thao túng sao?*](#act4_alone_skills_manipulative)

[Điều đó không khiến chúng ta *dễ bị thao túng hơn sao?*](#act4_alone_skills_manipulated)

[Nếu chúng ta vẫn thất bại thì sao?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Không phải những kẻ giết người hàng loạt có thể đọc được cảm xúc của nạn nhân là những kẻ rất giỏi "đồng cảm" sao?

`bb({ eyes:"annoyed" });`

b: Không phải Charles Manson đã có được bạn bè và ảnh hưởng đến mọi người sao?

`hong({ eyes:"annoyed", body:"chin" });`

h: Không, bạn nói đúng.

h: "Kỹ năng xã hội" chẳng có ý nghĩa gì nếu chúng ta không thực sự quan tâm *đến* mọi người.

`hong({ body:"normal" });`

h: Về cơ bản, đừng trở thành ^một tên khốn^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Cái đó nên trở thành chữ đề trên áp phích động viên.

`hong({ body:"shrug", mouth:"narrow" });`

h: Đừng Trở Thành ^Một Tên Khốn^™

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Chúng ta sẽ trở thành tấm thảm chùi chân chào đón, nói Làm ơn và Không có gì khi mọi người lau chân lên chúng ta!

`bb({ mouth:"scream", eyes:"scream" })`

b: Chúng ta sẽ hôn mông người khác nhiều đến nỗi trông như thể chúng ta đang tô son môi màu nâu vậy!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h:  Không, bạn nói đúng. "Kỹ năng xã hội" không chỉ là làm hài lòng người khác, mà còn phải là đặt ra *ranh giới*.

`hong( body:"one_up" });`

h: Chúng ta không thể mời người khác vào nhà mình, nếu chúng ta không có bức tường nào để chống đỡ ngôi nhà của mình.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Mà... re: hình ảnh tưởng tượng về màu son đó... *eo ôi??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Chúng ta có thể thất bại. Thực ra, chúng ta *sẽ* thất bại.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Và điều đó ổn thôi! Thất bại là cách bất kỳ ai cũng học được điều gì đó mới mẻ ngay từ đầu!

`hong({ body:"normal", eyes:"normal" });`

h: Vậy thì hãy cùng nhau thất bại, được chứ?

`bb({ eyes:"normal_r" });`

b: Chắc chắn rồi... trường hợp xấu nhất, chúng ta có thể bỏ trốn và có một danh tính mới.

`bb({ eyes:"normal" });`

h: Ừ mình nghĩ rằng ngày nay nó cũng chỉ tốn hai bitcoin.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Chúng ta có thể thử một số thí nghiệm!

`hong({ body:"chin" });`

h: Chúng ta có thể ping một người bạn để đi chơi, kết nối lại với một người bạn cũ, hoặc thậm chí chỉ trò chuyện với một nhân viên pha chế.

`hong({ body:"normal" });`

h: Mình nghĩ rằng chúng ta có thể thấy rằng chúng ta dễ mến hơn chúng ta nghĩ.

`bb({ eyes:"annoyed" });`

[Rủi đâu là những "chiến thắng" nhỏ, rẻ mạt thì sao?](#act4_alone_experiment_cheap)

[Rủi đâu đây là gánh nặng cho người khác thì sao?](#act4_alone_experiment_burden)

[Nhưng nói chuyện phiếm không phải là con người *thực* của chúng ta!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Nếu chúng ta nở một nụ cười hời hợt, chúng ta sẽ không bao giờ thực sự kết nối với bất kỳ ai,

`bb({ eyes:"super_sad" });`

b: *Nhưng* nếu chúng ta mở lòng, những người khác sẽ thấy tất cả những thứ bên trong hỗn loạn của chúng ta!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Lăn người ra.

b: Cái gì cơ.

`hong({body:"hands_1"})`

h: Khi chó muốn thể hiện tình yêu và lòng tin, chúng sẽ khiến bản thân dễ bị tổn thương bằng cách để lộ bụng.

`hong({body:"one_up"})`

h: Có thể chúng ta *chưa* đủ an toàn để trở nên quá dễ bị tổn thương, nhưng với đủ sự huấn luyện,

`hong({body:"normal", eyes:"surprise"})`

h: Một ngày nào đó chúng ta có thể cho mọi người thấy con người thật của mình – hoàn toàn lộn xộn, hoàn toàn là con người.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Tôi sẽ lăn qua nếu bạn cho tôi một miếng thức ăn.

`bb({ eyes:"normal", mouth:"normal" });`

h: Không.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Nói "xin chào" với nhân viên pha chế không hẳn là màn trình diễn giành huy chương vàng trong Thế vận hội Bươm Bướm Xã Hội.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Nó là dành cho *chúng ta!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: Trong đấu trường xã hội, chúng ta thậm chí không phải là hạng lông, chúng ta giống như... hạng quark.

`hong({ body:"normal", eyes:"normal" });`

h: Nếu chúng ta phải bắt đầu bằng những chiến thắng nhỏ và rẻ tiền, thì cứ thế đi. Phải leo lên bậc thang đầu tiên trước bậc thang thứ 1000.

b: Đúng vậy! Có lẽ sau khi nói "Xin chào", chúng ta có thể tiến tới nói...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Bạn khỏe không?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Không có gì nhiều!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Có lẽ nhân viên pha chế chỉ muốn pha cà phê thôi, chứ không muốn là một *thí nghiệm* để xem kỹ năng giao tiếp của chúng ta có tệ không.

`bb({ eyes:"annoyed" })`

h: Ừ thì, nếu hóa ra chúng ta *là* gánh nặng...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Biết thế cũng tốt!

`hong({ eyes:"normal" });`

h: Sau đó, chúng ta có thể học cách chủ động hỏi mọi người xem họ cảm thấy thoải mái với điều gì, để biết và tôn trọng ranh giới của người khác.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Bạn biết đấy, tất cả những "kỹ năng giao tiếp" ^rác rưởi^ mà chúng ta thấy trong các tờ rơi tư vấn.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Tôi muốn bảo vệ nhu cầu đạo đức của bạn, động lực để trở thành một người tốt hơn,

`bb({ eyes:"sad_d" })`

b: Nhưng sâu thẳm bên trong, chúng ta cảm thấy rằng về cơ bản... đã tan vỡ.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: Và đừng nói với tôi rằng chúng ta *không* bị hỗn loạn. Chúng ta đã nhảy từ một cái *mái nhà*.
{{/if}}

{{if !_.INJURED}}
b: Và đừng nói với tôi rằng chúng ta *không* bị hỗn loạn. Chúng ta đã suýt nhảy từ một cái *mái nhà*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Tôi không biết nữa, hơi đủ về việc *tôi* chọn điều gì để nói tiếp theo. *Bạn* sẽ nói gì, con người?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Một lần nữa, quay về bạn, con người. Bạn nghĩ sao?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Còn suy nghĩ gì nữa không, con người?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Vậy chúng ta tan vỡ rồi. Cùng sửa chúng ta nhé.](#act4_bad_fix)

[Vậy chúng ta tan vỡ rồi. Cùng chấp nhận nó nhé.](#act4_bad_accept)

[Cảm ơn bạn.](#act4_thanks) `_.thanks_for = "ổn định về đạo đức";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Chúng ta có thể dần dần xây dựng những thói quen tốt hơn, đưa cuộc sống của mình phù hợp hơn với những gì chúng ta coi trọng,

`hong({body:"one_up"});`

h: Và nếu cần, chúng ta có thể tìm kiếm sự giúp đỡ chuyên nghiệp – một nhà trị liệu hoặc cố vấn.

`hong({body:"normal"});`

h: Có nhiều cách để sửa chữa chúng ta.

[Rủi chúng ta không thể sửa chữa tất cả thì sao?](#act4_bad_fix_cant)

[Rủi chúng ta sửa chữa *quá* nhiều thì sao?](#act4_bad_fix_too_much)

[Chúng ta không đủ khả năng thuê chuyên gia.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Không, tôi đoán là bạn đúng.

h: Chúng ta không thể sửa chữa tất cả.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Àaaaa tôi biết là chúng ta sẽ luôn tan vỡ!

`hong({eyes:"surprise"});`

h: Nhưng ít nhất chúng ta có thể *ít* tan vỡ hơn.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Sẹo sẽ lành theo thời gian, nhưng chúng không bao giờ biến mất. Và điều đó không sao cả.

`bb({eyes:"annoyed_r"});`

b: Tôi đoán vậy. Bên cạnh đó,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Các vết sẹo rất *quyến rũ.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Xin đừng làm thế.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Thật buồn cười khi phải thừa nhận điều này, nhưng... một phần nào đó trong tôi *muốn* mắc chứng rối loạn này.

`bb({ eyes:"angry" })`

b: Ý tôi là, nếu không có nó, chúng ta sẽ *nhàm chán* phải không?

`bb({ eyes:"sad_r", body:"one_up" })`

b: Nếu không có chứng rối loạn này, nghệ thuật của chúng ta sẽ trở nên cũ kỹ và nhạt nhẽo phải không?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Nếu không có chứng rối loạn này, chúng ta sẽ không thể kết nối với những người bạn mắc chứng rối loạn này phải không?

`bb({ eyes:"sad", body:"chest" })`

b: Nếu chúng ta hài lòng với cuộc sống, chúng ta sẽ ngừng thúc đẩy bản thân làm những điều tuyệt vời sao?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Nếu chúng ta thậm chí còn sợ... "hết sợ"...

h: Tôi không nghĩ chúng ta sẽ hết sợ.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Ồ, tuyệt! Phù! Thật nhẹ nhõm!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Bác sĩ, tôi lo lắng rằng tôi phải trả 100 đô-la/giờ chỉ để nghe bác sĩ hỏi *điều đó khiến bác cảm thấy thế nào?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Ừm hứm. Và điều đó khiến bạn cảm thấy thế nào?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Không, đó là một nỗi lo hoàn toàn hợp lý.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: Và thật tệ khi dịch vụ chăm sóc sức khỏe  thần không phải là lựa chọn khả thi đối với nhiều người.

`hong({ eyes:"normal", mouth:"normal" });`

h: Tuy nhiên, vẫn có một số lựa chọn rẻ hoặc miễn phí:

`hong({ body:"chin" })`

h: Nhóm hỗ trợ, liệu pháp trực tuyến, trung tâm y tế dành cho sinh viên/phi lợi nhuận...

`hong({ body:"hands_1" })`

h: Xây dựng thói quen như thiền định, ngủ ngon, trò chuyện thường xuyên với bạn bè, học hỏi những điều mới...

`hong({ body:"hands_2" })`

h: Đến thư viện để mượn sách bài tập về liệu pháp tâm lý dựa trên bằng chứng...

`hong({ body:"one_up" })`

h: Có danh sách đầy đủ các nguồn tài nguyên ở cuối trò chơi này!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Chà, bức tường thứ tư *đó* không tồn tại lâu nhỉ.

`hong({ body:"point" });`

h: Một số thứ quan trọng hơn quy ước tường thuật. Chẳng hạn như sức khỏe  thần.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Ý tôi là, đó là những gì các nhà trị liệu nói đúng không? Chấp nhận mọi cảm xúc của bạn, ngay cả những cảm xúc tiêu cực?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Đợi đã.

["Chấp nhận" như trong *bỏ cuộc*?](#act4_bad_accept_give_up)

["Chấp nhận" như trong *đồng ý*?](#act4_bad_accept_approve)

["Chấp nhận" như trong *hiểu theo nghĩa đen*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Bạn có nghĩ Martin Luther King sẽ nói, "Chết tiệt, chúng ta không thể ngồi ở phía trước xe buýt, chúng ta hãy *chấp nhận* điều đó?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Tại sao Tổ hợp Công nghiệp Tự chăm sóc lại nghĩ rằng vẫy cờ trắng là một *chân lý sâu sắc?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Mình nghĩ các nhà trị liệu muốn nói "chấp nhận" những điều xấu như kiểu: thừa nhận chúng tồn tại và khó thay đổi,

h: Nhưng không nhất thiết phải từ bỏ cam kết thay đổi.

`bb({ eyes:"suspect" });`

b: Vậy thì các nhà trị liệu nên nói *thừa nhận*, không phải *chấp nhận*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Ừm, nghĩ lại thì "chấp nhận" hơi khó hiểu.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Vậy, tôi *thừa nhận* điều đó.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Như thể là *tốt* khi chúng ta bị tổn thương hay gì đó? Không!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Tất cả những nhà biên kịch Hollywood lãng mạn hóa bệnh tâm thần đều là đồ tồi!

`bb({ eyes:"angry", body:"two_up" });`

b: Mắc chứng rối loạn tâm thần *thật tệ!* Nó cướp đi *cuộc sống của mọi người!* Tại sao chúng ta phải "chấp nhận" điều đó?!

`bb({ body:"normal" });`

h: Tôi nghĩ các nhà trị liệu muốn nói đến "chấp nhận" cảm xúc của chúng ta theo nghĩa: hãy kiên nhẫn với chúng.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Giống như việc vật lộn trong cát lún khiến bạn chìm nhanh hơn, và giải pháp là kiên nhẫn nằm im,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Chống lại bạn, nỗi sợ của tôi, khiến tôi nhảy từ mái nhà xuống.
{{/if}}

{{if !_.INJURED}}
h: Chống lại bạn, nỗi sợ của tôi, khiến tôi suýt nhảy từ mái nhà xuống.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Thay vào đó, giải pháp là làm những gì chúng ta đang làm bây giờ – không phải là chống lại, mà là kiên nhẫn ở bên nhau.

`bb({ eyes:"annoyed" });`

b: Vậy thì họ nên nói *điều đó* thay vì một từ có vấn đề nào đó như "chấp nhận".

`hong({ body:"chin", eyes:"annoyed" });`

h: Ừ, nghĩ lại thì "chấp nhận" nghe tệ thật.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Tôi không chấp nhận "chấp nhận".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Nhưng chúng ta đã *biết* là bạn không nên hiểu tôi theo nghĩa đen!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Toàn bộ *vấn đề* là tôi muốn giúp bạn, nhưng tôi lại tệ trong việc sử dụng từ ngữ để làm như vậy!

`bb({ eyes:"sad", body:"normal" });`

h: Tôi nghĩ các nhà trị liệu muốn nói "chấp nhận" cảm xúc của bạn theo nghĩa: "đừng chống lại hoặc phớt lờ chúng".

`hong({ eyes:"surprise", body:"one_up" });`

h: Để lắng nghe bạn, làm việc *với* bạn, nhưng không coi những gì bạn nói là sự thật 100%.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Vậy thì các nhà trị liệu nên nói *điều đó* thay vì một từ mơ hồ gây nhầm lẫn nào đó như "chấp nhận".

`hong({ body:"chin", eyes:"annoyed" });`

h: Mình đoán là họ cũng tệ trong việc sử dụng từ ngữ.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Dù sao thì, bạn còn muốn trò chuyện về điều gì nữa không?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Vậy, còn điều gì nữa khiến trái tim bạn nặng trĩu không?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Tôi sợ chúng ta sẽ bị tổn thương.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Tôi sợ chúng ta sẽ cô đơn.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Tôi sợ chúng ta là người xấu.](#act4_bad)
{{/if}}

[Không, tôi ổn rồi.](#act4c_prelude)

# act4_something_else_2

h: Được rồi, mình nghĩ chúng ta đã nói về tất cả nỗi sợ của mình rồi.

b: Ừ, chỉ có ba nỗi sợ.

h: Ừ, chính xác là ba.

b: Tiện thật.

(#act4c)

# act4c_prelude

h: Trò chuyện vui vẻ lắm, cả đội.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Đây không phải là *trò chơi* đâu, bạn biết đấy.

`bb({eyes:"angry_d", body:"one_up"})`

b: Xây dựng mối quan hệ lành mạnh với cảm xúc của bạn không đơn giản chỉ là nhấp vào các nút trên màn hình.

`bb({eyes:"sad", body:"normal"})`

b: *Liệu* chúng ta có thực sự hòa hợp không?

b: *Liệu* chúng ta có thể làm việc cùng nhau, như một đội không?

`hong({eyes:"sad", body:"one_up"})`

h: Thì...

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: X-xin lỗi...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: C-c-cậu có phiền không nếu tớ ngồi ăn trưa cùng ?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Đây* là người bạn thích á? Tại sao họ lại ngồi một mình như một kẻ giết người hàng loạt tâm thần vậy?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Hỏi người bạn thích xem bạn có thể ngồi cùng họ không á? Bạn có biết chúng ta *đòi hỏi* đến cỡ nào không á?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Đây* là người bạn thích sao? Chúng ta đã phá vỡ sự yên bình và tĩnh lặng của họ! Chúng ta thật là một gánh nặng!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Ý tớ là- không sao nếu không, tớ chỉ...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Khoan, không phải mình thấy bạn ở bữa tiệc sao?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Ừ, tất nhiên rồi! Đến đây nào.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Xin lỗi, mình đang cần thời gian riêng tư.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Đúng là bạn đã nằm trên ghế dài! Ở bữa tiệc đầu tiên tôi đến...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Khi mình lên cơn hoảng loạn và đấm vào người chủ trì bữa tiệc.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Khi mình lên cơn hoảng loạn và chạy ra ngoài khóc lóc.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Đợi đã nào con người, chúng ta có thể đang khiến họ khó chịu.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: À, tôi không có ý định làm bạn bối rối!

`publish("act4", ["hong_to_alshire",4]);`

h2: Chỉ đang nhớ lại một khuôn mặt thân thiện, vậy á.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH TÔI BIẾT NGAY! HỌ LÀ BỆNH NHÂN TÂM THẦN NGUY HIỂM DO HOẢNG LOẠN!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH ẤN TƯỢNG ĐẦU TIÊN CHÚNG TA TẠO LÀ "CHỨNG KIẾN SỰ ĐAU THƯƠNG CỦA TÔI"! ĐIỀU ĐÓ CÓ NGHĨA LÀ HỌ GHÉT CHÚNG TA!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH CHÚNG TA ĐÃ KHIẾN AI ĐÓ NHỚ LẠI MỘT SỰ KIỆN ĐAU THƯƠNG. CHỈ CÓ MẶT CHÚNG TA ĐỀU LÀM TỔN THƯƠNG NGƯỜI KHÁC.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Đợi đã nào con người, họ có vẻ không thoải mái.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: À, tất nhiên là không có áp lực gì rồi!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Chỉ rằng, bạn có thể ngồi đây nếu bạn muốn.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: HỌ ĐANG *QUÁ* THÂN THIỆN! GIỐNG NHƯ TED BUNDY, KẺ GIẾT NGƯỜI HÀNG LOẠT!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: HỌ CHỈ ĐANG GIẢ VỜ TỐT THÔI! KHÔNG AI *THỰC SỰ* MUỐN GẦN CHÚNG TA!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH CHÚNG TA LUÔN LÀM NGƯỜI KHÁC CẢM THẤY NGẠI NGÙNG! CHÚNG TA LÀ MỘT VẾT NHƠ TRÊN TRÁI ĐẤT!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Đợi đã nào con người, chúng ta có thể đang khiến họ khó chịu.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: À, tôi không có ý thô lỗ đâu!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Tôi chỉ cần chút thời gian để xử lý cảm xúc của mình. Làm ơn đừng coi đó là sự từ chối cá nhân.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: HỌ ĐANG XỬ LÝ NHỮNG SUY NGHĨ BỆNH TẬT, VÔ LÝ NÀO?! NHỮNG MONG MUỐN TỐI TỐI ĐA ĐANG LẤP ĐẦY TRÁI TIM CỦA KẺ TÂM THẦN NÀY?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: CHÚNG TA ĐÃ BỊ TỪ CHỐI CÁ NHÂN! CHÚNG TA SẼ KHÔNG BAO GIỜ ĐƯỢC YÊU THƯƠNG!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: CHÚNG TA ĐÃ NGẮT CHẶN QUÁ TRÌNH XỬ LÝ CẢM XÚC CỦA HỌ! GIỜ ĐÂY HỌ SẼ BỊ TÂM LÝ MÃI MÃI VÀ ĐỀU LÀ LỖI CỦA CHÚNG TA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: CHẠY ĐI CHẠY ĐI CHẠY ĐI CHẠY ĐI CHẠY ĐI CHẠY ĐI CHẠY ĐI

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Hử. Kỳ lạ nhỉ. Không biết trong đầu họ đang nghĩ gì nữa.

`publish("act4", ["hong_closer", 2]);`

h: Dù sao thì, bạn vừa đang nói về gì vậy?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Ờ, tôi quên mất? Có gì đó về nhóm và việc?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Họ nói rằng bạn nên "làm hòa" với cảm xúc của mình, như thể cảm xúc của bạn là *tội phạm chiến tranh* vậy.

`publish("act4", ["bb_closer", 7]);`

b: Nhưng tôi muốn chúng ta tạo ra *nhiều* hơn là hòa bình đơn thuần! Tôi muốn chúng ta trở thành *đồng minh!*

`publish("act4", ["bb_closer", 3]);`

b: Tôi muốn trở thành một chú chó canh gác giỏi. Giống như đói và khát là những hồi chuông báo động cho nhu cầu thể chất của bạn,

`publish("act4", ["bb_closer", 8]);`

b: Tôi muốn trở thành hồi chuông báo động cho nhu cầu *tâm lý* của bạn – nhu cầu về sự an toàn, sự gắn bó, lòng tốt của bạn.

`publish("act4", ["bb_closer", 1]);`

b: Nhưng... Tôi tệ trong công việc của mình, vì vậy tôi cần bạn đào tạo tôi.

`publish("act4", ["bb_closer", 4]);`

b: Tôi không "luôn luôn hợp lệ" hay "luôn luôn phi lý". Tôi chỉ... cố gắng hết sức. Vậy nên, làm ơn,

`publish("act4", ["bb_closer", 30]);`

b: Giúp tôi giúp bạn nhé!

`publish("act4", ["bb_closer", 6]);`

b: Tuy nhiên, dạy một chú chó già những trò mới *sẽ* mất một thời gian. Có thể là *nhiều năm.*

`publish("act4", ["bb_closer", 3]);`

b: Và đôi khi tôi sẽ tái nghiện, tôi sẽ quay lại với những thói quen cũ của mình.

`publish("act4", ["bb_closer", 2]);`

b: Tôi sẽ sủa vào bóng tối. Tôi sẽ dọa bạn bằng những từ ngữ. Tôi thậm chí có thể cho bạn xem một số hình ảnh xâm phạm của... mọi thứ.

`publish("act4", ["bb_closer", 9]);`

b: Tôi xin lỗi! Tôi là một chú chó bị ngược đãi ở trại cứu hộ! Đôi khi những chú chó bị ngược đãi lại ị lên giường của bạn!

`publish("act4", ["bb_closer", 4]);`

b: Nhưng nếu bạn kiên nhẫn với tôi... và chỉ ở lại và ngồi với tôi...

`publish("act4", ["bb_closer", 8]);`

b: Có lẽ bạn có thể thuần hóa con sói này.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Chú chó ngoan.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Con người ngoan.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA BẠN VẪN ĂN MỘT MÌNH MƯỜI LĂM ĐIẾU THUỐC LÁ AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA BẠN VẪN KHÔNG HIỆU QUẢ KHI ĂN CHÚNG TA LÀ KÝ SINH TRÙNG CỦA XÃ HỘI AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA BẠN ĐANG ĂN NHIỀU BÁNH MÌ TRẮNG HƠN AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: YAP YAP YAP YAP YAP

(#credits)
