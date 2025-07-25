# Credimitro
Website for getting credit from all the banks and nbfcs 
import React from "react"; import { Button } from "@/components/ui/button";

export default function HomePage() { return ( <div className="min-h-screen bg-white text-gray-900"> {/* Hero Section */} <section className="bg-gradient-to-br from-yellow-100 via-white to-white py-20 text-center px-4"> <h1 className="text-4xl md:text-5xl font-bold mb-4">Tui chinta kor. Taka ta ami dekhe nebo.</h1> <p className="text-lg md:text-xl mb-6">Smart finance advice from your most trusted mitro.</p> <Button className="bg-yellow-400 hover:bg-yellow-500 text-black px-6 py-3 text-lg rounded-xl shadow">Book a Paid Consultation</Button> </section>

{/* Services Section */}
  <section className="py-16 px-6 bg-gray-50">
    <h2 className="text-3xl font-semibold text-center mb-12">Our Services</h2>
    <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-8 max-w-6xl mx-auto">
      {[
        "Personal Finance",
        "Loan Help",
        "Business Strategy",
        "Investment Advice",
      ].map((service) => (
        <div key={service} className="bg-white p-6 rounded-xl shadow hover:shadow-lg">
          <h3 className="text-xl font-semibold mb-2">{service}</h3>
          <p className="text-gray-600">Expert guidance for smart money decisions in {service.toLowerCase()}.</p>
        </div>
      ))}
    </div>
  </section>

  {/* About Section */}
  <section className="py-20 px-6 text-center bg-white">
    <h2 className="text-3xl font-bold mb-6">From Asansol to the World — Finance That Gets You</h2>
    <p className="max-w-2xl mx-auto text-gray-700">
      CediMitro is not just a consultancy — it's your friend in finance. Whether you're a student, small business owner, or dreamer from any corner of India, we're here to help you grow.
    </p>
  </section>

  {/* Testimonials Section */}
  <section className="bg-yellow-50 py-16 px-6">
    <h2 className="text-3xl font-semibold text-center mb-12">What People Say</h2>
    <div className="grid md:grid-cols-3 gap-6 max-w-6xl mx-auto">
      {[
        { name: "Rupam S.", feedback: "Tumi amar taka bachaile! Solid advice, bro." },
        { name: "Sahana D.", feedback: "First time consulting felt like talking to a friend." },
        { name: "Arjun M.", feedback: "Great for business ideas and cash flow planning." },
      ].map((t) => (
        <div key={t.name} className="bg-white p-6 rounded-xl shadow">
          <p className="text-gray-800 italic mb-2">"{t.feedback}"</p>
          <p className="text-sm font-semibold">– {t.name}</p>
        </div>
      ))}
    </div>
  </section>

  {/* Contact Section */}
  <section className="bg-gray-900 text-white py-16 px-6 text-center">
    <h2 className="text-3xl font-bold mb-4">Book Now via WhatsApp</h2>
    <p className="mb-6">Scan the UPI QR code or message us directly to confirm your consultation.</p>
    <Button className="bg-green-500 hover:bg-green-600 text-white px-6 py-3 text-lg rounded-xl shadow">Chat on WhatsApp</Button>
  </section>

  {/* Footer */}
  <footer className="bg-black text-white text-center py-6">
    <p>&copy; 2025 CediMitro. Proudly made in India 🇮🇳</p>
  </footer>
</div>

); }

