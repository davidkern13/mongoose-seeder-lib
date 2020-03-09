# mongoose-seeder-lib

Seed data into mongoose schemas

#### NPM
[npm library click here](https://www.npmjs.com/package/mongoose-seeder-lib)


#### Install
```
npm i --save mongoose-seeder-lib
```

#### Use

- import

```
const { createSeeder, dropDatabase } = require('mongoose-seeder-lib');
```

- create custom data to seed

```
const data = [
   {
        title: "Jordan 1 Retro High 85 Varsity Red",
        price: 679,
        currency: "USD",
        stock: 30,
    },
   {
        title: "Jordan 1 Retro High Yellow Ochre",
        price: 357,
        currency: "USD",
        stock: 15,
    },
    {
        title: "Jordan 1 Retro High Black Gym Red",
        price: 90,
        currency: "USD",
        stock: 107,
    },
];
```
#### Use createSeeder

```
/**
 * Seed passed data
 * @return { Promise } 
 */

const res = await createSeeder(data, schema);
```

![Alt Text](https://i.gyazo.com/fc7cb436b81ecd7c1d03b43954d2bf3d.gif)


#### Use dropDatabase

```
/**
 * Remove all data from table
 * @return { Promise } 
 */

const res = await dropDatabase(schema);
```

![Alt Text](https://i.gyazo.com/6e6d21c38dd7deb60e3dab0545966553.gif)


