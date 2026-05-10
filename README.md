
export default function WomensHealthWebsite() {
  return (
    <div className="min-h-screen bg-[#f8f3f1] text-[#5b4a4a] font-sans">
      {/* Hero Section */}
      <section className="px-6 py-16 md:px-20 flex flex-col md:flex-row items-center justify-between gap-10">
        <div className="max-w-xl">
          <p className="uppercase tracking-[0.3em] text-sm text-[#b38b8b] mb-4">
            Women’s Health Physiotherapy
          </p>

          <h1 className="text-5xl md:text-6xl font-light leading-tight mb-6">
            Restore Your Core <br />
            After Birth
          </h1>

          <p className="text-lg leading-8 text-[#6b5b5b] mb-8">
            A gentle 6-week recovery program designed to help women heal
            diastasis recti, strengthen the pelvic floor, and regain confidence
            after pregnancy.
          </p>

          <div className="flex gap-4 flex-wrap">
            <button className="bg-[#c89d9d] hover:bg-[#b88a8a] text-white px-8 py-4 rounded-2xl text-lg shadow-lg transition">
              Download Program
            </button>

            <button className="border border-[#c89d9d] px-8 py-4 rounded-2xl text-lg hover:bg-[#efe1de] transition">
              Learn More
            </button>
          </div>
        </div>

        <div className="relative">
          <div className="w-[320px] h-[320px] rounded-full bg-[#ead7d3] absolute blur-3xl opacity-70"></div>

          <img
            src="https://images.unsplash.com/photo-1584515933487-779824d29309?q=80&w=1200&auto=format&fit=crop"
            alt="Women Physiotherapy"
            className="relative w-[340px] h-[430px] object-cover rounded-[2rem] shadow-2xl"
          />
        </div>
      </section>

      {/* Features */}
      <section className="px-6 md:px-20 py-14 bg-white">
        <div className="text-center mb-14">
          <h2 className="text-4xl font-light mb-4">What’s Included</h2>
          <p className="text-[#7b6b6b] text-lg">
            Everything you need for a safe and guided recovery journey.
          </p>
        </div>

        <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
          {[
            {
              title: '6-Week Exercise Plan',
              desc: 'Step-by-step weekly exercises for safe recovery.',
            },
            {
              title: 'Pelvic Floor Training',
              desc: 'Gentle breathing and pelvic floor activation exercises.',
            },
            {
              title: 'Weekly Checklists',
              desc: 'Track your progress and stay motivated every week.',
            },
            {
              title: 'Common Mistakes Guide',
              desc: 'Learn what to avoid during healing.',
            },
            {
              title: 'Recovery Tips',
              desc: 'Daily habits that support faster recovery.',
            },
            {
              title: 'Professional Guidance',
              desc: 'Created by a women’s health physiotherapist.',
            },
          ].map((item, index) => (
            <div
              key={index}
              className="bg-[#f8f3f1] p-8 rounded-3xl shadow-sm hover:shadow-lg transition"
            >
              <h3 className="text-2xl mb-3">{item.title}</h3>
              <p className="text-[#6f5f5f] leading-7">{item.desc}</p>
            </div>
          ))}
        </div>
      </section>

      {/* About */}
      <section className="px-6 md:px-20 py-16 flex flex-col md:flex-row gap-12 items-center">
        <img
          src="https://images.unsplash.com/photo-1516549655669-df8a8f5f5c5d?q=80&w=1200&auto=format&fit=crop"
          alt="Physiotherapist"
          className="w-full md:w-[420px] rounded-[2rem] shadow-xl"
        />

        <div className="max-w-2xl">
          <h2 className="text-4xl font-light mb-6">About The Program</h2>

          <p className="text-lg leading-8 text-[#6b5b5b] mb-6">
            This program was designed to support women during their postpartum
            recovery journey using evidence-based physiotherapy principles.
          </p>

          <p className="text-lg leading-8 text-[#6b5b5b]">
            Whether you are struggling with abdominal separation, weak core
            muscles, or pelvic floor symptoms, this guide helps you rebuild
            strength safely and gradually.
          </p>
        </div>
      </section>

      {/* CTA */}
      <section className="px-6 md:px-20 py-20 text-center bg-[#ead7d3]">
        <h2 className="text-5xl font-light mb-6">
          Start Your Healing Journey Today
        </h2>

        <p className="text-xl text-[#6b5b5b] mb-10 max-w-2xl mx-auto leading-8">
          Small consistent steps create long-term healing and confidence.
        </p>

        <button className="bg-[#5b4a4a] text-white px-10 py-5 rounded-2xl text-xl shadow-xl hover:opacity-90 transition">
          Buy Now – $19
        </button>
      </section>

      {/* Footer */}
      <footer className="py-8 text-center text-[#8b7b7b] bg-white text-sm">
        © 2026 Women’s Health Physiotherapy • Strong From Within
      </footer>
    </div>
  );
}
