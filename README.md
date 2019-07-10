2019/07/10 indexとnewを変更

index.html

<div class="wrapper">
      <!-- Left View -->
    <div class="LeftView">

      <iframe src="/tweets/new" frameborder="0" width="50%" height="100%"></iframe>
    </div>
    <!-- Right View -->
    <div class="RigthView">
        <div class="show">
          <% @tweets.each do |tweet| %>
            <p><%= tweet.body %></p>
            <%= link_to 'Show',tweet%>
          <% end %>
        </div>
    </div>

</div>

new.html

<h1>Create a new tweet</h1>

<!-- ADD -->
<%= render "form", tweet: @tweet %>
<!-- ADD -->

<!-- REMOVE -->
 <%= form_with(model: @tweet, local: true) do |form| %>

  <div>
    
  </div>
<% end %>
<!-- REMOVE -->
