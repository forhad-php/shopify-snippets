- Login to shopify admin
- Online store → Theme → Edit Code
- Section → main-collection-product-grid.liquid

```JS
<h2 class="rich-text__heading"><span>{{ collection.title }}</span></h2>
<div class="main">
  {% assign handle = "GIFTS FOR WIFE" %}
    {% case handle %}
      {% when "GIFTS FOR WIFE" %}
        <p>The best gift a husband can give his wife is the gift of love and commitment. Then comes jewelry, which is one of the most preferred items for maximum girls.</p>
        <p>So, if you are looking to surprise your wife with an unpredictable gift, consider gifting a beautiful necklace, bracelet, or earrings of your choice with your heartfelt personalized message.</p>

      {% when "Gifts For Girlfriend" %}
        <p>When it comes to gifting jewelry to your lovely girlfriend, you can’t go wrong. Show your affection and token of love with our beautiful jewelry gifts for your girlfriend, like necklaces, bracelets, or earrings.</p>
        <p>Fetch The Love has some unique jewelry collections to gift your girlfriend, and we also let you convey your feelings by sharing your customized message on our gift box that she will cherish forever.</p>

      {% when "Gifts For Future Wife" %}
      <p>Gifting jewelry to your future wife is always a great idea that can never go wrong. From birthdays to anniversaries and anything in between, we have got the perfect gifts for your future wife here.</p>
      
      {% else %}
      Collection not found.

      {% endcase %}
</div>

```

- To console log any object
```JS
<script>console.log({{ collection | json }});</script>
```
