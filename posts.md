## All Posts
 <ul>
   {% for post in site.posts %}
     <li>
       <a href="{{ post.url }}">{{ post.title }}</a>
     </li>
   {% endfor %}
 </ul>

 ## Categories 
 <ul>
 {% for category in site.categories %}
   <p>{{ category[0] }}</p>
     {% for post in category[1] %}
       <li><a href="{{ post.url }}">{{ post.title }}</a></li>
     {% endfor %}
 {% endfor %}
</ul>

 ## Tags 
 {% for tag in site.tags %}
   <p>{{ tag[0] }}</p>
   <ul>
     {% for post in tag[1] %}
       <li><a href="{{ post.url }}">{{ post.title }}</a></li>
     {% endfor %}
   </ul>
 {% endfor %}
