Image Search Abstraction Layer
================================

--------------------------
User stories:
--------------------------

- I can get the image URLs, alt text and page urls for a set of images relating to a given search string.

- I can paginate through the responses by adding a ?offset=2 parameter to the URL.

- I can get a list of the most recently submitted search strings.


--------------------------
Example usage:
--------------------------

https://imagesearch-hr.glitch.me/api/imagesearch/lolcats

https://imagesearch-hr.glitch.me/api/imagesearch/lolcats%20funny?offset=2

https://imagesearch-hr.glitch.me/api/latest/imagesearch/

--------------------------
Example query output:
--------------------------

[{
  "url":"http://www.lolcats.com/",
  "snippet":"LOLCats - Funny cat pictures",
  "thumbnail":"https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcR8hkDSbxoKKNODgZDDb_nZyi6WEMvIH3x-bbcRmXrGwdDTQ397HuQg2cc",
  "context":"http://www.lolcats.com/images/u/13/39/tastegood.jpg"
},{
  "url":"http://icanhas.cheezburger.com/lolcats/page/2",
  "snippet":"Lolcats - Page 2 - LOL at Funny Cat Memes - Funny cat pictures with ...",
  "thumbnail":"https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcRSuIYwEnII4RE88oyX4OoEjDK8dKl5oPF5QqbYjFUPA-Vo6ZJGgOeBA6I",
  "context":"https://i.chzbgr.com/original/9144193536/h42903CF2/"
},{
  "url":"http://www.lolcats.com/gallery/popular.html",
  "snippet":"LOLCats - Popular - Page 1",
  "thumbnail":"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ6rarLCszoBV_aSyhAntVH3EU4KZjme7fNuOlkm0QCV8XKI5auoa0L",
  "context":"http://www.lolcats.com/images/u/12/24/thumbs/lolcatsdotcom-found-it.jpg"
},{
  "url":"http://icanhas.cheezburger.com/tag/lolcats",
  "snippet":"I Can Has Cheezburger? - lolcats - Funny Animals Online ...",
  "thumbnail":"https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcRza_bsj303h6uEceJ2mWk0GRCgDL0X853Ntgi2wK4G8n5oA1TjBxrz6qA",
  "context":"https://i.chzbgr.com/thumb800/5212933/h7DC508AD/"
},{
  "url":"https://www.facebook.com/LOLCatsOfficial/",
  "snippet":"Lolcats.com - Home | Facebook",
  "thumbnail":"https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcQdiY3zPj56p9X3tJXhIUxhGqsmVOmKQ_0M97CEdbe5shEmfgG2OY2ZEN-w",
  "context":"https://lookaside.fbsbx.com/lookaside/crawler/media/?media_id=664599473550715"
},{
  "url":"http://icanhas.cheezburger.com/",
  "snippet":"I Can Has Cheezburger? - Funny Animals Online - Cheezburger",
  "thumbnail":"https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcSm1z-seHTvVDmXlynPiV3V_QpB3MbVnB-ba4Rtr0oi5b3dgkRPfikx39I",
  "context":"https://i.chzbgr.com/thumb800/5217541/h77317FDA/"
},{
  "url":"https://itunes.apple.com/us/app/lolcats-funny-cat-pics/id289278734?mt=8",
  "snippet":"LOLCats - Funny Cat Pics on the App Store",
  "thumbnail":"https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcTe5OfM1JfTRmRisdsAobbrGL6aFyGk_PnDQTnmMaRrev_nc__i198HWIQ",
  "context":"https://is4-ssl.mzstatic.com/image/thumb/Purple118/v4/81/2e/69/812e695a-410d-93b2-5308-c88841838426/AppIconLOLCatsFree-1x_U007emarketing-85-220-0-4.jpeg/1200x630bb.jpg"
},{
  "url":"http://mentalfloss.com/article/521963/school-book-pioneered-funny-cat-pics-100-years-lolcats",
  "snippet":"The School Book That Pioneered Funny Cat Pics 100 Years Before ...",
  "thumbnail":"https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcThxfUpNivcBcz4tZQhYZdYRpntcs0uquWF6LezEPQ1kzVOGuFN2amqtaE",
  "context":"http://images.mentalfloss.com/sites/default/files/styles/mf_image_16x9/public/521963-kittenscatspublicdomain.jpg?itok=QomlkSKU"
},{
  "url":"https://www.urbandictionary.com/define.php?term=lolcat",
  "snippet":"Urban Dictionary: lolcat"},{"url":"http://www.smosh.com/smosh-pit/photos/30-best-lol-cats-ever","snippet":"30 Best LOLcats Ever | SMOSH",
  "thumbnail":"https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcQ_T1TVnVzdgg0dtHayvEqe1pSmo8kBHzBt8s0MeC5pNm5ehGbMx99lLEQ",
  "context":"http://cdn.smosh.com/sites/default/files/styles/large/public/smosh-pit/122010/lolcat-thumb_1.jpg?itok=TSukEiWV"
}]

--------------------------
Example latest output:
--------------------------

[{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:41:42.355Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:41:53.545Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:42:33.074Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:42:40.696Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:43:20.954Z"
},{
  "term":"lolcats%20sad",
  "when":"2018-04-04T08:44:41.321Z"
},{
  "term":"lolcats%20sad",
  "when":"2018-04-04T08:44:48.540Z"
},{
  "term":"lolcats%20sad",
  "when":"2018-04-04T08:44:51.810Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:45:11.974Z"
},{
  "term":"lolcats",
  "when":"2018-04-04T08:45:16.015Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:45:21.865Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:45:25.301Z"
},{
  "term":"lolcats%20funny",
  "when":"2018-04-04T08:45:29.919Z"
}]

--------------------------
Made by [hr](https://github.com/hrego/)