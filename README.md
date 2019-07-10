style.scss変更
/* View関係 */
body {
    margin: 0px;
    padding: 0px;
    background: #FAE8DD;
}

ul {
	list-style-type: none;
	margin: 0;
	padding: 0;
	overflow: hidden;
	background-color: #1b2538;
}
li {
	float: left;
	border-right: 1px solid #bbbbbb;
}
li:last-child {
	border-right: none;
}
li a {
	display: block;
	color: white;
	text-align: center;
	text-decoration: none;
  padding-top:10px;
  padding-bottom:10px;
  padding-left:24px;
  padding-right:24px;
}
li a:hover:not(.active) {
	background-color: #a9bce2;
}
.active {
	background-color: #da3c41;
}
.last{
  float: inherit;
}

.site-header{
    position: fixed;
    width: 100%;
}
.font{
  text-align: center;
  font-family: 'times new roman';
}

.wrapper{
  display: flex;
}

.column{
    height: 100%;
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


/<header class = "site-header">
/  <ul class = "font">
/	   <li><a class="active" href="#home">Home</a></li>
/	   <li><a href="#news">Tweet</a></li>
/	   <li><a href="#contact">View</a></li>
/     <li><a href="#about">About</a></li>
/     <li class = "last"><a>GameHistry</a></li>
/
/  </ul>
/</header>
/
/<body>
/  <div class="wrapper">
/        <!-- Left View -->
/        <div class="LeftView">
/          <iframe src="/tweets/new" frameborder="0" width="50%" height="100%"></iframe>
/        </div>
/
/  <!-- Right View -->
/  <div class="RigthView">
/    <div class="show">
/      <% @tweets.each do |tweet| %>
/      <p><%= tweet.body %></p>
/      <%= link_to 'Show',tweet%>
/      <% end %>
/    </div>
/  </div>
/
/</div>
/</body>
/インデックス.html

