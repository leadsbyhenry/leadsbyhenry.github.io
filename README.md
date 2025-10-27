// src/App.jsx
import React from "react";
import { BrowserRouter as Router, Routes, Route, Link } from "react-router-dom";

function Navbar() {
  return (
    <nav className="flex justify-between items-center p-6 bg-white shadow-md">
      <h1 className="text-2xl font-bold text-blue-600">NovaScale AI</h1>
      <ul className="flex gap-6 text-gray-700">
        <li><Link to="/">Home</Link></li>
        <li><Link to="/services">Services</Link></li>
        <li><Link to="/case-studies">Case Studies</Link></li>
        <li><Link to="/about">About</Link></li>
        <li><Link to="/contact" className="text-blue-600 font-semibold">Contact</Link></li>
      </ul>
    </nav>
  );
}

function Home() {
  return (
    <section className="flex flex-col items-center justify-center text-center min-h-screen bg-gray-50 p-6">
      <h2 className="text-4xl md:text-5xl font-bold text-blue-600 mb-4">Unlock 10× Growth with AI</h2>
      <p className="text-gray-700 mb-6 max-w-xl">
        We help service businesses automate content, ads, and leads — saving 20+ hours per week and boosting revenue within 30 days.
      </p>
      <a href="/contact" className="bg-blue-600 text-white px-6 py-3 rounded-lg font-semibold hover:bg-blue-700 transition">
        Book Your Free AI Growth Audit
      </a>
    </section>
  );
}

function Services() {
  const services = [
    { title: "AI Marketing Automation", desc: "Automate ads, content, and social media for maximum ROI." },
    { title: "AI Content Studio", desc: "Generate high-converting copy, images, and videos instantly." },
    { title: "Lead Generation AI", desc: "Find, engage, and convert clients automatically." }
  ];

  return (
    <section className="p-12 bg-white">
      <h2 className="text-3xl font-bold text-center text-blue-600 mb-8">Our Services</h2>
      <div className="grid md:grid-cols-3 gap-8">
        {services.map((s, i) => (
          <div key={i} className="p-6 border rounded-lg shadow hover:shadow-lg transition">
            <h3 className="text-xl font-semibold mb-2">{s.title}</h3>
            <p className="text-gray-700">{s.desc}</p>
          </div>
        ))}
      </div>
    </section>
  );
}

function CaseStudies() {
  const cases = [
    { title: "Real Estate Ads AI", result: "+35% leads in 30 days" },
    { title: "Fitness Studio Automation", result: "Saved 15 hrs/week, +25% clients" },
    { title: "E-commerce Campaigns", result: "+40% ROAS using AI" }
  ];

  return (
    <section className="p-12 bg-gray-50">
      <h2 className="text-3xl font-bold text-center text-blue-600 mb-8">Case Studies</h2>
      <div className="grid md:grid-cols-3 gap-8">
        {cases.map((c, i) => (
          <div key={i} className="p-6 border rounded-lg shadow hover:shadow-lg transition">
            <h3 className="text-xl font-semibold mb-2">{c.title}</h3>
            <p className="text-gray-700">{c.result}</p>
          </div>
        ))}
      </div>
    </section>
  );
}

function About() {
  return (
    <section className="p-12 bg-white text-center">
      <h2 className="text-3xl font-bold text-blue-600 mb-4">About NovaScale AI</h2>
      <p className="text-gray-700 max-w-2xl mx-auto">
        NovaScale AI is a premium AI marketing and automation agency. Our mission is to help service businesses save time, increase revenue, and scale using cutting-edge AI tools. We combine automation, analytics, and creative AI content to deliver measurable results.
      </p>
    </section>
  );
}

function Contact() {
  return (
    <section className="p-12 bg-gray-50 text-center">
      <h2 className="text-3xl font-bold text-blue-600 mb-4">Contact Us</h2>
      <p className="text-gray-700 mb-6">Book your free AI growth audit today.</p>
      <form className="max-w-lg mx-auto flex flex-col gap-4">
        <input type="text" placeholder="Full Name" className="p-3 border rounded"/>
        <input type="email" placeholder="Email Address" className="p-3 border rounded"/>
        <textarea placeholder="Your Message" className="p-3 border rounded"></textarea>
        <button className="bg-blue-600 text-white px-6 py-3 rounded-lg font-semibold hover:bg-blue-700 transition">Send Message</button>
      </form>
    </section>
  );
}

export default function App() {
  return (
    <Router>
      <Navbar />
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="/services" element={<Services />} />
        <Route path="/case-studies" element={<CaseStudies />} />
        <Route path="/about" element={<About />} />
        <Route path="/contact" element={<Contact />} />
      </Routes>
    </Router>
  );
}



