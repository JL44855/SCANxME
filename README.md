export default function ScanxmeLandingPage() { return ( <div className="min-h-screen bg-black text-white overflow-hidden"> {/* HERO */} <section className="relative flex flex-col items-center justify-center min-h-screen px-6 text-center"> <div className="absolute inset-0 bg-gradient-to-b from-green-500/10 to-black"></div>

{/* Rings */}
    <div className="absolute w-[700px] h-[700px] rounded-full border border-green-500/20 animate-pulse"></div>
    <div className="absolute w-[500px] h-[500px] rounded-full border border-green-500/30"></div>
    <div className="absolute w-[300px] h-[300px] rounded-full border-4 border-green-400 shadow-[0_0_80px_rgba(34,197,94,0.8)]"></div>

    <div className="relative z-10 max-w-5xl">
      <h1 className="text-6xl md:text-8xl font-black tracking-tight">
        SCAN<span className="text-green-400">x</span>ME
      </h1>

      <p className="mt-8 text-3xl md:text-5xl font-bold leading-tight">
        Ton vêtement <br />
        <span className="text-green-400">est ton profil.</span>
      </p>

      <p className="mt-8 text-gray-300 text-lg max-w-2xl mx-auto leading-relaxed">
        SCANxME connecte les objets du monde réel à l'identité numérique.
        Scanne. Découvre. Connecte.
      </p>

      <div className="mt-10 flex flex-col md:flex-row gap-4 justify-center">
        <button className="bg-green-500 hover:bg-green-400 text-black font-bold px-8 py-4 rounded-2xl text-lg transition-all shadow-[0_0_30px_rgba(34,197,94,0.5)]">
          Télécharger l'application
        </button>

        <button className="border border-green-500 text-green-400 hover:bg-green-500/10 px-8 py-4 rounded-2xl text-lg transition-all">
          Découvrir le concept
        </button>
      </div>
    </div>
  </section>

  {/* HOW IT WORKS */}
  <section className="py-32 px-6 max-w-7xl mx-auto">
    <div className="text-center mb-20">
      <h2 className="text-5xl font-black">
        Comment ça marche
      </h2>
      <p className="mt-6 text-gray-400 text-lg">
        Le monde réel devient interactif.
      </p>
    </div>

    <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
      {[
        {
          title: '1. Porte ton objet',
          desc: 'Ajoute ton manteau, sneakers ou accessoires à ton profil public.'
        },
        {
          title: '2. Fais-toi scanner',
          desc: 'Les gens découvrent ton profil et les objets que tu portes.'
        },
        {
          title: '3. Vends ou expose',
          desc: 'Tes objets peuvent être achetés, négociés ou simplement montrés.'
        }
      ].map((item, i) => (
        <div
          key={i}
          className="bg-zinc-900 border border-green-500/20 rounded-3xl p-8 hover:border-green-400 transition-all hover:shadow-[0_0_30px_rgba(34,197,94,0.2)]"
        >
          <div className="w-14 h-14 rounded-full bg-green-500/20 border border-green-500 flex items-center justify-center text-green-400 font-bold text-xl mb-6">
            {i + 1}
          </div>

          <h3 className="text-2xl font-bold mb-4">{item.title}</h3>
          <p className="text-gray-400 leading-relaxed">{item.desc}</p>
        </div>
      ))}
    </div>
  </section>

  {/* MARKETPLACE */}
  <section className="py-32 px-6 bg-zinc-950 border-y border-green-500/10">
    <div className="max-w-7xl mx-auto grid md:grid-cols-2 gap-20 items-center">
      <div>
        <h2 className="text-5xl font-black leading-tight">
          Plus qu'une <span className="text-green-400">marketplace.</span>
        </h2>

        <p className="mt-8 text-gray-400 text-lg leading-relaxed">
          SCANxME transforme les objets physiques en identités numériques interactives.
          Chaque vêtement, sneaker ou accessoire peut être montré, partagé,
          scanné ou vendu directement dans la vraie vie.
        </p>

        <div className="mt-10 space-y-4">
          {[
            'Objets interactifs',
            'Profil public intelligent',
            'QR code unique',
            'Marketplace vivant',
            'Négociation en temps réel',
            'Historique des objets'
          ].map((feature, i) => (
            <div key={i} className="flex items-center gap-4">
              <div className="w-3 h-3 bg-green-400 rounded-full"></div>
              <span className="text-lg">{feature}</span>
            </div>
          ))}
        </div>
      </div>

      <div className="relative flex items-center justify-center">
        <div className="absolute w-[450px] h-[450px] rounded-full border border-green-500/20"></div>
        <div className="absolute w-[300px] h-[300px] rounded-full border border-green-500/30"></div>

        <div className="relative z-10 bg-black border border-green-500/30 rounded-[40px] p-6 w-[320px] shadow-[0_0_80px_rgba(34,197,94,0.15)]">
          <div className="rounded-3xl bg-zinc-900 p-6">
            <div className="w-24 h-24 rounded-full bg-green-500/20 mx-auto mb-6"></div>

            <h3 className="text-center text-2xl font-bold">@scanxme</h3>
            <p className="text-center text-gray-400 mt-2">Profil public</p>

            <div className="mt-8 grid grid-cols-2 gap-4">
              {[50, 120, 80, 200].map((price, i) => (
                <div
                  key={i}
                  className="bg-black border border-green-500/20 rounded-2xl p-4"
                >
                  <div className="h-24 rounded-xl bg-zinc-800 mb-3"></div>
                  <p className="font-bold">{price}€</p>
                </div>
              ))}
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  {/* FINAL CTA */}
  <section className="py-32 px-6 text-center relative">
    <div className="absolute inset-0 bg-green-500/5"></div>

    <div className="relative z-10 max-w-4xl mx-auto">
      <h2 className="text-5xl md:text-7xl font-black leading-tight">
        Le monde réel. <br />
        <span className="text-green-400">Connecté.</span>
      </h2>

      <p className="mt-8 text-gray-400 text-xl leading-relaxed">
        SCANxME crée une nouvelle manière d'interagir avec les personnes,
        les objets et le monde physique grâce au scan et à l'identité numérique.
      </p>

      <button className="mt-12 bg-green-500 hover:bg-green-400 text-black font-bold px-10 py-5 rounded-2xl text-xl transition-all shadow-[0_0_40px_rgba(34,197,94,0.5)]">
        Rejoindre SCANxME
      </button>
    </div>
  </section>
</div>

) }