Learn to use meteor.js
<a href="slides.com/hsin-chieh/meteor-js"><h1>Slides:Meteor基本簡介</h1></a>

第一步驟
```    
    1.meteor create meteor
    2.cd meteor
    3.meteor  (In cloud 9 you should use : meteor --port $IP:$PORT  )
 ```           
第二步驟
```    
        加入 bootstrap underscore
        4.meteor add twbs:bootstrap
        5.meteor add underscore

    6.mkdir client public lib 
    7.copy the css file in client/stylesheets/style.css
    8.copy main.html in client
    9.copy templates and posts/posts_item/list/js 
```
    現在有一個靜態的模板資料了!
```    
    10.update the new code on posts_list.html
    11.create post_item.js
    12.create lib/collections/posts.js
    13.create server/fixtures.js
```
    試試看在瀏覽器的console裡面使用
    ```
            Posts.insert({
              title: 'Meteor Docs',
              author: 'Tom Coleman', 
              url: 'http://docs.meteor.com'
            });
    ```        
第四步驟:加入討論區
    ```
        14.meteor remove autopublish //刪除自動枚舉
        15.copy main.js
        16.meteor add iron:router
    ```    
       
第五步驟:
    加入登入
    ```
        meteor add ian:accounts-ui-bootstrap-3
        17.meteor add accounts-password
        18.copy client/templates/application/layout.html
        19.copy client/templates/includes/header.html
    ```    