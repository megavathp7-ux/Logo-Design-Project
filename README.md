<div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10">
      {logos.map((logo, index) => (
        <div
          key={index}
          className="bg-gray-900 border border-gray-800 rounded-3xl shadow-2xl overflow-hidden hover:scale-105 transition-transform duration-300"
        >
          <div className="flex items-center gap-2 px-5 py-4 border-b border-gray-800 bg-black">
            <div className="w-3 h-3 rounded-full bg-red-500"></div>
            <div className="w-3 h-3 rounded-full bg-yellow-400"></div>
            <div className="w-3 h-3 rounded-full bg-green-500"></div>
            <span className="ml-4 text-sm text-gray-400 font-mono">
              github/logo-design
            </span>
          </div>

          <div className="p-10 text-center">
            <div
              className={`w-28 h-28 mx-auto rounded-3xl bg-gradient-to-br ${logo.gradient} flex items-center justify-center text-5xl font-bold shadow-xl mb-6`}
            >
              {logo.symbol}
            </div>

            <h2 className="text-3xl font-bold mb-2">{logo.name}</h2>

            <p className="text-gray-400 mb-8">{logo.tagline}</p>

            <div className="flex justify-center gap-3 flex-wrap">
              <span className="px-4 py-2 bg-gray-800 rounded-full text-sm">
                Minimal
              </span>
              <span className="px-4 py-2 bg-gray-800 rounded-full text-sm">
                Modern
              </span>
              <span className="px-4 py-2 bg-gray-800 rounded-full text-sm">
                Startup
              </span>
            </div>
          </div>
        </div>
      ))}
    </div>

    <div className="mt-16 bg-gray-900 border border-gray-800 rounded-3xl p-8 shadow-xl">
      <h2 className="text-3xl font-bold mb-6">GitHub Deployment Guide</h2>

      <div className="bg-black rounded-2xl p-5 font-mono text-green-400 text-sm overflow-x-auto leading-8">
        git init
        <br />
        git add .
        <br />
        git commit -m "Add logo design showcase"
        <br />
        git branch -M main
        <br />
        git remote add origin YOUR_GITHUB_REPOSITORY
        <br />
        git push -u origin main
      </div>

      <div className="mt-6 text-gray-400 leading-relaxed">
        Upload this project to GitHub and deploy it easily using GitHub
        Pages, Vercel, or Netlify.
      </div>
    </div>
  </div>
</div>
