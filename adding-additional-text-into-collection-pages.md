- Login to shopify admin
- Online store → Theme → Edit Code
- Section → main-collection-product-grid.liquid

```React
<h2 class="rich-text__heading"><span>{{ collection.title }}</span></h2>
<div class="main">
  {% assign handle = collection.handle %}
    {% case handle %}
      {% when "gift-for-wife" %}
        <p>Content about Gift For Wife.</p>

      {% when "gifts-for-girlfriend" %}
        <p>Content about Gift For GF.</p>

      {% when "gifts-for-future-wife" %}
      <p>Content about Gift For FF.</p>
      
      {% else %}
      Collection not match.

      {% endcase %}
</div>

```

- To console log any object
```HTML
<script>console.log({{ collection | json }});</script>
```
