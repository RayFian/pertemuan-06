This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.tsx`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.ts`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.


|  | Pemrograman Berbasis Framework 2024 |
|--|--|
| NIM |  2141720260|
| Nama |  Raynor Herfian Iqbal Fawwaz |
| Kelas | TI - 3I |

## Praktikum 1
![alt text](image.png)

The nextJS project importing the css style and also resources from bootstrap that provided from the Javascript

## Praktikum 2
### Soal 1
![alt text](image-1.png)

![alt text](image-2.png)

based on the result we can access the login and logout message. When we press the button under the card-body we the function handleAuth will alternate between login and logout

### Soal 2
Line 25
```
parse('<div class="alert alert-success">Yay, berhasil login!!!</div>'),
```

Line 30
```
parse('<div class="alert alert-dark">Anda telah logout!</div>'),
```

Parse command refers to done the elements as JSX elements with background. If we didn't use the parse command it will be normal HTML strings


## Praktikum 3
![alt text](image-3.png)

![alt text](image-4.png)

In this practicum we asked to create counter as an implementation of how to manage state using Redux in NextJS.

## Pertanyaan

1. Apa kegunaan dari kode ini import { useEffect } from "react"; Pada file pages/_app.tsx? jelaskan

### Jawaban
The purpose of the code import { useEffect } from "react"; in the file pages/_app.tsx is to bring in the useEffect function from the React module. This function helps manage side effects in functional components. It's useful for things like handling actions when a component mounts, updates, or unmounts.

2. Jika pada file pages/_app.tsx kita tidak menggunakan useEffect menghapus baris 3, dan baris 9-11, apa yang akan terjadi?

### Jawaban
If lines 3 and 9-11, which contain the usage of useEffect, are removed from the file pages/_app.tsx, there won't be any noticeable effect on the _app.tsx component. However, if the _app.tsx component is used to manage something that requires side effects, such as setting metadata on page changes, then that functionality will be lost.

3. Mengapa di react/nextjs penulisan tag html untuk class, harus diganti menjadi className?

### Jawaban
In React/Next.js, using className instead of class in HTML tags is done because JSX, the syntax extension used by React, conflicts with the JavaScript keyword class. To avoid confusion between HTML attributes and class usage in JavaScript, HTML attribute class is replaced with className in JSX.

4. Apakah store pada nextjs bisa menyimpan banyak redux reducer?

### Jawaban
In Next.js, a store typically refers to state management, especially when using Redux. The Redux store in Next.js can store multiple reducers. The store.js file is where the Redux store is usually defined and configured. It includes creating the store, combining reducers, and applying middleware if needed. This file is important as it serves as the central place for state management in Next.js applications using Redux.

5. Jelaskan kegunaan dari file store.js!

### Jawaban
In the file pages/login.tsx, the code const { isLogin } = useSelector((state) => state.auth); is used to retrieve the value isLogin from the Redux state stored in the auth reducer. This indicates that the login.tsx component uses Redux to manage the user's login status. The value isLogin is likely used to control the display or behavior of the component based on the user's login status.

6. Pada file pages/login.tsx, apa maksud dari kode ini ?
const { isLogin } = useSelector((state) => state.auth);

### Jawaban
In the file pages/counter.tsx, the code const {totalCounter} = useSelector((state) => state.counter); is used to fetch the value totalCounter from the Redux state stored in the counter reducer. This indicates that the counter.tsx component uses Redux to manage state related to counting. The value totalCounter is likely used to display the total count or perform other operations related to counting within the component.

7. Pada file pages/counter.tsx, apa maksud dari kode ini?
const {totalCounter} = useSelector((state) => state.counter);

### Jawaban
In the file pages/counter.tsx, the code const {totalCounter} = useSelector((state) => state.counter); means that it's using the useSelector hook from the React Redux library to access the totalCounter value from the Redux state. This line is extracting the totalCounter property from the state.counter object.