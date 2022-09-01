# NeoBase Client

Javascript client for [neobase](https://neobase.ir)

### install

```bash
npm i @neobase/client
```

### Usage

First get your project name from [NeoBase](https://neobase.ir), if you don't have a project yet, register and create one, it's free!

```javascript
import { getClient } from '@neobase/client'

const client = getClient('your-project-name', { baseurl: 'https://neobase.darkube.app' })

//create a collection object
const Todos = client.Collection('todos')

//create a document
const { data, status } = await client.create({ name: 'update the docs', done: false })

//fetch data
const { data, status } = await client.find()
```

### Documents

Please read NeoBase documents at [Docs](https://neobase.ir/docs).
