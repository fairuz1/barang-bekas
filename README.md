# Barang Bekas Backend

Features breakdown:

-   ### Admin:
    -   [x] add product
    -   [x] add category
    -   [x] edit product
    -   [x] edit category
    -   [x] delete product
    -   [x] delete category
    -   [x] edit admin profile
-   ### API:
    -   [x] get all products
    -   [x] get products by category
    -   [x] search products by keyword
    -   [x] get product detail by id
    -   [x] get admin data

## API Endpoint

### GET All Products

#### Endpoint

```
https://barbek.rf.gd/api/product
```

#### Payload

```
{
  "status": 200,
  "message": "get all product success",
  "data": [
    {
      "id": "1",
      "name": "Laptop Infinix Inbook X3",
      "description": "Laptop Infinix Inbook X1, \r\nkeren\r\ndengan intel core i3",
      "image": "https://barbek.rf.gd/assets/img/1667633140-infinix-inbook-x1_169.jpeg",
      "price": "5900000",
      "stock": "89",
      "weight": "1300",
      "category_id": "1"
    },
    {
      "id": "2",
      "name": "Inifinix Hot 9",
      "description": "Smartphone Inifinix Hot 9, ram 4 rom 128, mediatek helio a22",
      "image": "https://barbek.rf.gd/assets/img/inifinix-hot9.jpg",
      "price": "1599000",
      "stock": "14",
      "weight": "300",
      "category_id": "2"
    }
  ]
}
```

### GET Detail Product by Id

#### Endpoint

```
https://barbek.rf.gd/api/product?id={id}
```

#### Payload

```
{
  "status": 200,
  "message": "success get product by id",
  "data": [
    {
      "id": "1",
      "name": "Laptop Infinix Inbook X3",
      "description": "Laptop Infinix Inbook X1, \r\nkeren\r\ndengan intel core i3",
      "image": "https://barbek.rf.gd/assets/img/1667633140-infinix-inbook-x1_169.jpeg",
      "price": "5900000",
      "stock": "89",
      "weight": "1300",
      "category_id": "1"
    }
  ]
}
```

### GET Products by Category id

#### Endpoint

```
https://barbek.rf.gd/api/product?category={category_id}
```

#### Payload

```
{
  "status": 200,
  "message": "get product by category success",
  "category": "laptop",
  "data": [
    {
      "id": "1",
      "name": "Laptop Infinix Inbook X3",
      "description": "Laptop Infinix Inbook X1, \r\nkeren\r\ndengan intel core i3",
      "image": "https://barbek.rf.gd/assets/img/1667633140-infinix-inbook-x1_169.jpeg",
      "price": "5900000",
      "stock": "89",
      "weight": "1300",
      "category_id": "1"
    }
  ]
}
```

### Search Products

#### Endpoint

```
https://barbek.rf.gd/api/product?search={keyword}
```

#### Payload

```
{
  "status": 200,
  "message": "search product success",
  "query": "i",
  "data": [
    {
      "id": "1",
      "name": "Laptop Infinix Inbook X3",
      "description": "Laptop Infinix Inbook X1, \r\nkeren\r\ndengan intel core i3",
      "image": "https://barbek.rf.gd/assets/img/1667633140-infinix-inbook-x1_169.jpeg",
      "price": "5900000",
      "stock": "89",
      "weight": "1300",
      "category_id": "1"
    },
    {
      "id": "2",
      "name": "Inifinix Hot 9",
      "description": "Smartphone Inifinix Hot 9, ram 4 rom 128, mediatek helio a22",
      "image": "https://barbek.rf.gd/assets/img/inifinix-hot9.jpg",
      "price": "1599000",
      "stock": "14",
      "weight": "300",
      "category_id": "2"
    }
  ]
}
```

### GET all categories

#### Endpoint

```
https://barbek.rf.gd/api/category
```

#### Payload

```
{
  "status": 200,
  "message": "get all category success",
  "data": [
    {
      "id": "1",
      "name": "laptop",
      "image": "https://barbek.rf.gd/assets/img/1667634191-laptop.jpg"
    },
    {
      "id": "2",
      "name": "smartphone",
      "image": "https://barbek.rf.gd/assets/img/hp.jpg"
    }
  ]
}
```

### GET category by id

#### Endpoint

```
https://barbek.rf.gd/api/category?id={category_id}
```

#### Payload

```
{
  "status": 200,
  "message": "success get category by id",
  "data": [
    {
      "id": "1",
      "name": "laptop",
      "image": "https://barbek.rf.gd/assets/img/1667634191-laptop.jpg"
    }
  ]
}
```

### GET Admin Data

#### Endpoint

```
https://barbek.rf.gd/api/admin
```

#### Payload

```
{
  "status": 200,
  "message": "success get admin data",
  "data": [
    {
      "username": "admin",
      "email": "admin@mail.com",
      "wa": "62895331850313",
      "role": "admin"
    }
  ]
}
```
