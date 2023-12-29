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

1. Clone the repository to the local system either by ZIP File or Using the following git command:
```
git clone https://github.com/aniru-dh21/hotel-management.git
```

2. Change the present working directory to the repository `cd hotel-management` and install dependencies using the npm or yarn or pnpm:
```
npm install
# or
yarn install
# or
pnpm install
```

3. Set environment variables to run the application in root directory by creating `.env` file:
```
STRIPE_WEBHOOK_SECRET=<Your_Secret_key>
NEXT_PUBLIC_SANITY_PROJECT=<Your_Secret_key>
NEXT_PUBLIC_SANITY_DATASET=<Your_Secret_key>
GITHUB_CLIENT_ID=<Your_Secret_key>
GITHUB_CLIENT_SECRET=<Your_Secret_key>
GOOGLE_CLIENT_ID=<Your_Secret_key>
GOOGLE_CLIENT_SECRET=<Your_Secret_key>
NEXTAUTH_SECRET=<Your_Secret_key>
SANITY_STUDIO_TOKEN=<Your_Secret_key>
STRIPE_SECRET_KEY=<Your_Secret_key>
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=<Your_Secret_key>
```

4. After setting up `.env` file run the following commad to run the development server:
```
npm run dev
# or
yarn dev
# or
pnpm dev
```

5. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.
