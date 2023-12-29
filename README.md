# Hotel Management Site with Next.js, Sanity.io, and Tailwind CSS

Creating a seamless and intuitibe hotel management site is essential for enhancing the guest experience and streamlining and administrative tasks. Our project aims to achieve this by leveraging cutting-edge technologies to deliver a responsive and visually appealing platform. Through thoughtful design and user-friendly interfaces, we intend to provide both guests and hotel staff with an efficient and enjoyable interaction. The emphasis is on creating a dynamic website that not only showcases the hotel's offerings but also facilitates easy booking, management, and communication.

## Core Technologies Used

- **Next.js**: A React framework that enables functionality such as server-side rendering and generating static websites, making your application faster and more efficient.

- **React**: A JavaScript for building user interfaces, known for its efficiency and flexibility in creating dynamic, high-performing web applications.

- **Sanity.io**: A platform for structured content that comes with an open-source editing environment that allows you to manage and deliver digital content globally.

- **Tailwind CSS**: A utility-first CSS framework for rapidly building custom designs, providing low-level utility classes to build bespoke designs without leaving your HTML.

- **Stripe**: An online payment processing platform that's highly flexible and integrates easily with various web applications for secure and efficient financial transactions.

## Highlights of the Project

- **CRUD Operations with Sanity.IO**: Manage hotel rooms effectively with full create, read, update, and delete capabilities.

- **Room Booking & Review**: Implement features for booking hotel rooms and providing room reviews.

- **Payment Processing**: Integrate Stripe for secure and efficient checkout experiences.

- **React Context for UI Themes**: Master the use of React Context for dynamic theme switching.

- **Advanced Search and Authentication**: Implement a robust search feature and secure user authentication.

- **TypeScript and useSwr Hook**: Enhancing project with TypeScript for better code management and use the useSwr hook for data fetching.

## File Directory Structure

```
hotel-management
├── README.md
├── next-auth.types.ts
├── next.config.js
├── package-lock.json
├── package.json
├── postcss.config.js
├── public
│   ├── images
│   │   ├── hero-1.jpeg
│   │   ├── hero-2.jpeg
│   │   └── hero-3.jpeg
│   ├── next.svg
│   └── vercel.svg
├── sanity.config.ts
├── schemas
│   ├── account.ts
│   ├── booking.ts
│   ├── hotelRoom.ts
│   ├── index.ts
│   ├── review.ts
│   ├── user.ts
│   └── verificationToken.ts
├── src
│   ├── app
│   │   ├── (cms)
│   │   │   ├── layout.tsx
│   │   │   └── studio
│   │   │       └── [[...index]]
│   │   │           └── page.tsx
│   │   ├── (web)
│   │   │   ├── auth
│   │   │   │   └── page.tsx
│   │   │   ├── error.tsx
│   │   │   ├── favicon.ico
│   │   │   ├── globals.css
│   │   │   ├── layout.tsx
│   │   │   ├── loading.tsx
│   │   │   ├── page.tsx
│   │   │   ├── rooms
│   │   │   │   ├── [slug]
│   │   │   │   │   └── page.tsx
│   │   │   │   └── page.tsx
│   │   │   └── users
│   │   │       └── [id]
│   │   │           └── page.tsx
│   │   └── api
│   │       ├── auth
│   │       │   └── [...nextauth]
│   │       │       └── route.ts
│   │       ├── room-reviews
│   │       │   └── [id]
│   │       │       └── route.ts
│   │       ├── sanity
│   │       │   └── signUp
│   │       │       └── route.ts
│   │       ├── stripe
│   │       │   └── route.ts
│   │       ├── users
│   │       │   └── route.ts
│   │       └── webhook
│   │           └── route.ts
│   ├── components
│   │   ├── AuthProvider
│   │   │   └── AuthProvider.tsx
│   │   ├── BackDrop
│   │   │   └── BackDrop.tsx
│   │   ├── BookRoomCta
│   │   │   └── BookRoomCta.tsx
│   │   ├── Chart
│   │   │   └── Chart.tsx
│   │   ├── CountUpNumber
│   │   │   └── CountUpNumber.tsx
│   │   ├── FeaturedRoom
│   │   │   └── FeaturedRoom.tsx
│   │   ├── Footer
│   │   │   └── Footer.tsx
│   │   ├── Gallery
│   │   │   └── Gallery.tsx
│   │   ├── Header
│   │   │   └── Header.tsx
│   │   ├── HeroSection
│   │   │   ├── ClientComponent.tsx
│   │   │   ├── HeroSection.tsx
│   │   │   └── ServerComponent.tsx
│   │   ├── HotelPhotoGallery
│   │   │   └── HotelPhotoGallery.tsx
│   │   ├── NewsLetter
│   │   │   └── NewsLetter.tsx
│   │   ├── PageSearch
│   │   │   └── PageSearch.tsx
│   │   ├── Rating
│   │   │   └── Rating.tsx
│   │   ├── RatingModal
│   │   │   └── RatingModal.tsx
│   │   ├── RoomCard
│   │   │   └── RoomCard.tsx
│   │   ├── RoomReview
│   │   │   └── RoomReview.tsx
│   │   ├── Search
│   │   │   └── Search.tsx
│   │   ├── Table
│   │   │   └── Table.tsx
│   │   ├── ThemeProvider
│   │   │   └── ThemeProvider.tsx
│   │   └── Toast
│   │       └── Toast.tsx
│   ├── context
│   │   └── themeContext.ts
│   ├── libs
│   │   ├── apis.ts
│   │   ├── auth.ts
│   │   ├── sanity.ts
│   │   ├── sanityQueries.ts
│   │   └── stripe.ts
│   ├── middleware.ts
│   └── models
│       ├── booking.ts
│       ├── review.ts
│       ├── room.ts
│       └── user.ts
├── tailwind.config.ts
└── tsconfig.json
```

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
