tweet.css 変更

/* View関係 */
body {
    margin: 10px;
    padding: 10px;
    background: #fff;
}
.wrapper{
  display: flex;
}

.column{
    height: 100vh;
    width: 100%;

    display: flex;
    text-align: center;
    align-items: center;
    justify-content: center;
}

.LeftView{

  width: 50%;
  background: url(../image/back.jpg) no-repeat top center;

}

.RigthView{
    /* background: blue no-repeat top center; */
    width: 50%;
}

index.html 変更
<div class="wrapper">
      <!-- Left View -->

    <div class="new LeftView">
      <%= link_to  "New Tweet", new_tweet_path %>
      <iframe src="/tweets/new" frameborder="0"></iframe>
    </div>
    <!-- Right View -->
    <div class="show RigthView">
        <div class="show">
          <% @tweets.each do |tweet| %>
            <p><%= tweet.body %></p>
            <%= link_to 'Show',tweet%>
          <% end %>
        </div>
    </div>

</div>
