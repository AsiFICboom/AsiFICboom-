// pages/index.js
import Head from 'next/head';
import Image from 'next/image';
import Link from 'next/link';

export default function Home() {
  return (
    <div className="min-h-screen bg-gray-100">
      <Head>
        <title>AsiFIC Boom - Premier Event Space</title>
      </Head>
      <header className="bg-blue-600 text-white p-4">
        <h1 className="text-2xl font-bold">AsiFIC Boom</h1>
        <p className="text-sm">Your Business, Our Space</p>
      </header>
      <main className="p-4">
        <section className="mb-8">
          <h2 className="text-xl font-semibold mb-4">About Us</h2>
          <p className="text-gray-700">Best located 4-storey commercial building with lift and parking space.</p>
        </section>
        <section className="mb-8">
          <h2 className="text-xl font-semibold mb-4">Location</h2>
          <div className="h-64 bg-gray-300">Google Map Integration</div>
        </section>
        <section className="mb-8">
          <h2 className="text-xl font-semibold mb-4">Gallery</h2>
          <div className="grid grid-cols-2 gap-4">
            <Image src="/building.jpg" alt="Building" width={300} height={200} />
            <Image src="/hall.jpg" alt="Hall" width={300} height={200} />
          </div>
        </section>
        <Link href="/booking">
          <a className="bg-orange-500 text-white px-4 py-2 rounded">Book Now</a>
        </Link>
      </main>
    </div>
  );
}# AsiFICboom-
