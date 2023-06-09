﻿# Python-Web-scraping-Json
 
# Help shoppers find product “alternates”

When you go shopping, you may have noticed that some of the products are available in “alternate choices” of colors, prints, etc. 

You have to use your AI skills to write a program that will find alternates of the same product in a given e-commerce store. Write a function named `FindAlternateGroups()` that takes store_domain as the parameter and returns links of products that are alternates of each other in an array. There will be many product alternates arrays in a store, so return all of them in a JSON.

```json
[
{"product alternates":['product_link_1', 'product_link_3']},
{"product alternates":['product_link_5', 'product_link_11', 'product_link_7']}
]
```

You can use any existing library or API to implement the solution.

Here is an example:

Boys Next Door Apparel Co is a popular Hong-Kong based Menswear & Lifestyle Store. 

You can visit their store at [boysnextdoor-apparel.co](https://www.boysnextdoor-apparel.co/)

You can find all products at [/collections/all](https://www.boysnextdoor-apparel.co/collections/all)

You can find all products data in JSON format by paginating through this link: [/collections/all/products.json?page=1](https://www.boysnextdoor-apparel.co/collections/all/products.json?page=1)

The following two products [BEAMS Two Pocket Sweater Navy](https://www.boysnextdoor-apparel.co/products/beams-two-pocket-sweater-navy) and [BEAMS Two Pocket Sweater White](https://www.boysnextdoor-apparel.co/products/beams-two-pocket-sweater-white) are alternate choices of the same product, so your function should return their product link in the same array. 

```json
[
{"product alternates":['https://www.boysnextdoor-apparel.co/products/beams-two-pocket-sweater-white', 'https://www.boysnextdoor-apparel.co/products/beams-two-pocket-sweater-navy']}
]
```

![Untitled](https://laser-comb-669.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fa7b5afcc-0889-46c8-abe7-8ecbbc1cff00%2FUntitled.png?id=c98a9eb1-77b8-4abc-9e6e-f225e365d7a5&table=block&spaceId=614642c7-f11f-4106-87d2-d8a3e0ea1b80&width=2000&userId=&cache=v2)

Other stores for testing your program:

[https://www.woolsboutiqueuomo.com/collections/all](https://www.woolsboutiqueuomo.com/collections/all)

[https://sartale2022.myshopify.com/collections/all](https://sartale2022.myshopify.com/collections/all)

[https://berkehome.pl/collections/all](https://berkehome.pl/collections/all)

[https://glamaroustitijewels.com/collections/all](https://glamaroustitijewels.com/collections/all)

[https://lampsdepot.com/collections/all](https://lampsdepot.com/collections/all)

[https://kitchenoasis.com/collections/all](https://kitchenoasis.com/collections/all)
