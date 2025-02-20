## BUILD & RUN CODE

**Pull Code**

`git clone https://github.com/khuyennv/nguyen_van_khuyen`

`cd nguyen_van_khuyen`

**Build & Run**

`yarn install`

`yarn dev`

## Test

**Get all items:**
`curl http://localhost:7000/api/menu/items -i`

**Get an item:**
`curl http://localhost:7000/api/menu/items/2 -i`

**Add an item:**

```
curl -X POST -H 'Content-Type: application/json' -d '{
  "name": "Salad",
  "price": 499,
  "description": "Fresh",
  "image": "/salad-sm.png"
}' http://localhost:7000/api/menu/items -i

```

**Update an item:**

```
curl -X PUT -H 'Content-Type: application/json' -d '{
  "name": "Spicy Pizza",
  "price": 599,
  "description": "Blazing Good",
  "image": "whatabyte_pizza-sm.png"
}' http://localhost:7000/api/menu/items/2 -i
```

**Delete an item:**

```
curl -X DELETE http://localhost:7000/api/menu/items/2 -i
```
