import { useState } from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

type ArticleId = 'onderwijs' | 'zorg' | 'pensioen' | 'werk' | 'migratie' | '';

export default function Home() {
  const [currentArticle, setCurrentArticle] = useState<ArticleId>('');

  const showArticle = (id: ArticleId) => {
    setCurrentArticle(id);
    window.scrollTo({ top: 0, behavior: 'smooth' });
  };

  const articles = [
    {
      id: 'onderwijs' as const,
      title: 'Onderwijs: Gratis bijles voor gelijke kansen',
      excerpt: 'In 2040 krijgen kinderen uit minder rijke gezinnen gratis bijles. Een revolutie in onderwijstoegankelijkheid.',
      icon: '📘',
      color: 'blue',
      impact: 'Afgenomen 🎉',
      impactType: 'positive',
      fullContent: 'In 2040 krijgen kinderen uit minder rijke gezinnen gratis bijles. Ouders en scholen zien verbeterde resultaten. Minister Jacobs zegt: "Iedereen verdient gelijke kansen."',
      image: 'https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&h=800',
      reactions: [
        { party: 'Links', sentiment: 'Positief', icon: '💚', description: 'Partijen juichen de maatregel toe als belangrijke stap naar gelijke kansen voor alle kinderen.' },
        { party: 'Midden', sentiment: 'Steunend', icon: '💛', description: 'Gematigd positief, met focus op effectieve implementatie en meetbare resultaten.' },
        { party: 'Rechts', sentiment: 'Kritisch over kosten', icon: '💸', description: 'Zorgen over de financiële haalbaarheid en effectiviteit van overheidsinterventie.' }
      ]
    },
    {
      id: 'zorg' as const,
      title: 'Zorg: Wie betaalt, wordt sneller geholpen',
      excerpt: 'Het nieuwe zorgsysteem introduceert betaalde spoedzorg. Efficiëntie of ongelijkheid?',
      icon: '🏥',
      color: 'green',
      impact: 'Toegenomen ⚠️',
      impactType: 'warning',
      fullContent: 'In het nieuwe systeem kunnen mensen sneller geholpen worden als ze bijbetalen. Dit verkort wachttijden voor sommigen, maar roept vragen op over eerlijkheid en solidariteit.',
      image: 'https://images.unsplash.com/photo-1551601651-2a8555f1a136?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&h=800',
      reactions: [
        { party: 'Links', sentiment: 'Oneerlijk', icon: '🚫', description: 'Sterke kritiek op het creëren van een tweeklassensysteem in de zorg.' },
        { party: 'Midden', sentiment: 'Verdeeld', icon: '⚖️', description: 'Begrip voor efficiency, maar zorgen over toegankelijkheid voor iedereen.' },
        { party: 'Rechts', sentiment: 'Vrije markt', icon: '👍', description: 'Ondersteuning voor marktmechanismen die efficiency en keuze bevorderen.' }
      ]
    },
    {
      id: 'pensioen' as const,
      title: 'Pensioen: 65 is het nieuwe 70',
      excerpt: 'De pensioenleeftijd daalt naar 65 jaar. Meer vrijheid voor werknemers, maar hoe houdbaar is dit?',
      icon: '👵',
      color: 'purple',
      impact: 'Verlaagd voor mensen met zware beroepen 👍',
      impactType: 'positive',
      fullContent: 'De pensioenleeftijd gaat van 70 naar 65 jaar. Veel mensen zijn blij met meer vrije jaren, maar er zijn zorgen over belastinginkomsten voor toekomstige generaties.',
      image: 'https://images.unsplash.com/photo-1559028006-448665bd7c7f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2073&h=800',
      reactions: [
        { party: 'Links', sentiment: 'Blij', icon: '😄', description: 'Enthousiast over meer rust voor werknemers na een lang arbeidsleven.' },
        { party: 'Midden', sentiment: 'Voorzichtig positief', icon: '🙂', description: 'Steun voor de maatregel, maar wel aandacht voor duurzame financiering.' },
        { party: 'Rechts', sentiment: 'Kritisch', icon: '🤨', description: 'Zorgen over de financiële impact en gevolgen voor toekomstige generaties.' }
      ]
    },
    {
      id: 'werk' as const,
      title: 'Werk: Robots nemen het over',
      excerpt: 'Automatisering transformeert de arbeidsmarkt. Oplossing voor personeelstekorten of bedreiging voor werkgelegenheid?',
      icon: '🤖',
      color: 'orange',
      impact: 'Risico voor lager opgeleiden ⚙️',
      impactType: 'warning',
      fullContent: 'Robots zijn overal: in supermarkten, horeca en magazijnen. Door personeelstekorten biedt technologie uitkomst, maar er is zorg over verloren banen voor laagopgeleiden.',
      image: 'https://images.unsplash.com/photo-1485827404703-89b55fcc595e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&h=800',
      reactions: [
        { party: 'Links', sentiment: 'Willen omscholing', icon: '🧑‍🏫', description: 'Pleiten voor massale investeringen in herscholing en nieuwe vaardigheden.' },
        { party: 'Midden', sentiment: 'Balanceren', icon: '🤹', description: 'Zoeken naar evenwicht tussen technologische vooruitgang en sociale bescherming.' },
        { party: 'Rechts', sentiment: 'Innovatie stimuleren', icon: '🚀', description: 'Focus op het bevorderen van technologische innovatie en concurrentiekracht.' }
      ]
    },
    {
      id: 'migratie' as const,
      title: 'Migratie: Europa bereidt zich voor',
      excerpt: 'Nieuwe migratiegolven vereisen Europese samenwerking. Hoe balanceert Nederland solidariteit en controle?',
      icon: '🌍',
      color: 'teal',
      impact: 'Druk op voorzieningen 🏘️',
      impactType: 'neutral',
      fullContent: 'Meer vluchtelingen door oorlog en armoede. Nederland werkt samen met de EU en stelt strengere regels op. De discussie over verdeling blijft actueel.',
      image: 'https://images.unsplash.com/photo-1569025743873-ea3a9ade89f9?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&h=800',
      reactions: [
        { party: 'Links', sentiment: 'Hulp bieden', icon: '❤️', description: 'Benadrukken humanitaire plicht en het belang van internationale solidariteit.' },
        { party: 'Midden', sentiment: 'Europese samenwerking', icon: '🤝', description: 'Focussen op gezamenlijke Europese aanpak en eerlijke verdeling.' },
        { party: 'Rechts', sentiment: 'Strenger beleid', icon: '🔒', description: 'Pleiten voor strengere controles en beperkingen op migratiestromen.' }
      ]
    }
  ];

  const getColorClasses = (color: string) => {
    const colorMap = {
      blue: 'bg-blue-100 text-blue-600',
      green: 'bg-green-100 text-green-600',
      purple: 'bg-purple-100 text-purple-600',
      orange: 'bg-orange-100 text-orange-600',
      teal: 'bg-teal-100 text-teal-600'
    };
    return colorMap[color as keyof typeof colorMap] || 'bg-gray-100 text-gray-600';
  };

  const getImpactClasses = (type: string) => {
    const impactMap = {
      positive: 'bg-green-50 border-l-4 border-green-400',
      warning: 'bg-orange-50 border-l-4 border-orange-400',
      neutral: 'bg-gray-50 border-l-4 border-gray-400'
    };
    return impactMap[type as keyof typeof impactMap] || 'bg-gray-50 border-l-4 border-gray-400';
  };

  return (
    <div className="bg-gray-50 text-gray-900 antialiased min-h-screen">
      <noscript>
        <div className="bg-red-100 border border-red-400 text-red-700 px-4 py-3 rounded text-center">
          ⚠️ Deze site werkt beter met JavaScript ingeschakeld.
        </div>
      </noscript>

      {/* Header Section */}
      <header className="bg-white shadow-sm border-b border-gray-200">
        <div className="max-w-7xl mx-auto">
          {/* Hero Image Section */}
          <div className="relative h-64 md:h-80 overflow-hidden">
            <img 
              src="https://images.unsplash.com/photo-1477959858617-67f85cf4f1df?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2044&h=800" 
              alt="Futuristische skyline van Nederland in 2040" 
              className="w-full h-full object-cover"
            />
            <div className="absolute inset-0 bg-gradient-to-t from-black/60 via-black/20 to-transparent"></div>
            <div className="absolute bottom-0 left-0 right-0 p-6 md:p-8 text-white">
              <div className="max-w-4xl mx-auto">
                <h1 className="text-3xl md:text-5xl font-bold mb-3">📰 Het Nieuws in 2040</h1>
                <p className="text-lg md:text-xl font-light opacity-90">Utopie of Dystopie? Een blik op de toekomst van Nederland</p>
              </div>
            </div>
          </div>
        </div>
      </header>

      {/* Navigation */}
      <nav className="bg-white border-b border-gray-200 sticky top-0 z-40 shadow-sm" role="navigation" aria-label="Hoofdmenu">
        <div className="max-w-7xl mx-auto">
          <div className="flex flex-wrap justify-center md:justify-start items-center px-4 py-3 space-x-1 md:space-x-6">
            <Button
              variant="ghost"
              size="sm"
              onClick={() => showArticle('')}
              className="text-gray-700 hover:text-blue-600 hover:bg-gray-50 transition-colors duration-200"
            >
              📊 Overzicht
            </Button>
            {articles.map(article => (
              <Button
                key={article.id}
                variant="ghost"
                size="sm"
                onClick={() => showArticle(article.id)}
                className="text-gray-700 hover:text-blue-600 hover:bg-gray-50 transition-colors duration-200"
              >
                {article.icon} {article.id.charAt(0).toUpperCase() + article.id.slice(1)}
              </Button>
            ))}
          </div>
        </div>
      </nav>

      {/* Main Content */}
      <main className="max-w-6xl mx-auto px-4 py-8">
        
        {/* Article Overview (Default View) */}
        {currentArticle === '' && (
          <div className="article-transition">
            <div className="mb-8">
              <h2 className="text-2xl md:text-3xl font-bold text-gray-900 mb-4">Hoofdartikelen</h2>
              <p className="text-lg text-gray-600 leading-relaxed">Ontdek hoe Nederland er in 2040 uitziet. Van onderwijs tot gezondheidszorg, van werk tot migratie - elk artikel belicht een cruciaal aspect van onze toekomstige samenleving.</p>
            </div>

            <div className="grid gap-6 md:gap-8">
              {articles.map(article => (
                <Card key={article.id} className="bg-white shadow-sm border border-gray-200 overflow-hidden card-hover-effect">
                  <CardContent className="p-6 md:p-8">
                    <div className="flex items-start space-x-4">
                      <div className="flex-shrink-0">
                        <div className={`w-12 h-12 ${getColorClasses(article.color)} rounded-lg flex items-center justify-center text-2xl`}>
                          {article.icon}
                        </div>
                      </div>
                      <div className="flex-1">
                        <h3 className="text-xl font-semibold text-gray-900 mb-2">{article.title}</h3>
                        <p className="text-gray-600 mb-4 leading-relaxed">{article.excerpt}</p>
                        <Button
                          variant="link"
                          onClick={() => showArticle(article.id)}
                          className="news-blue hover:text-blue-700 p-0 h-auto font-medium transition-colors duration-200"
                        >
                          Lees meer <span className="ml-2">→</span>
                        </Button>
                      </div>
                    </div>
                  </CardContent>
                </Card>
              ))}
            </div>
          </div>
        )}

        {/* Individual Articles */}
        {articles.map(article => (
          currentArticle === article.id && (
            <article key={article.id} className="article-transition">
              <div className="max-w-4xl mx-auto">
                <div className="mb-8">
                  <Button
                    variant="link"
                    onClick={() => showArticle('')}
                    className="news-blue hover:text-blue-700 p-0 h-auto font-medium mb-6 transition-colors duration-200"
                  >
                    ← Terug naar overzicht
                  </Button>
                  <div className="flex items-center space-x-3 mb-4">
                    <div className={`w-8 h-8 ${getColorClasses(article.color)} rounded-lg flex items-center justify-center text-lg`}>
                      {article.icon}
                    </div>
                    <span className={`text-sm font-medium uppercase tracking-wide ${article.color === 'blue' ? 'text-blue-600' : article.color === 'green' ? 'text-green-600' : article.color === 'purple' ? 'text-purple-600' : article.color === 'orange' ? 'text-orange-600' : 'text-teal-600'}`}>
                      {article.id === 'zorg' ? 'Gezondheidszorg' : 
                       article.id === 'werk' ? 'Werk & Technologie' : 
                       article.id === 'migratie' ? 'Migratie & Europa' : 
                       article.id.charAt(0).toUpperCase() + article.id.slice(1)}
                    </span>
                  </div>
                  <h1 className="text-3xl md:text-4xl font-bold text-gray-900 mb-4">{article.title.split(': ')[1]}</h1>
                  <p className="text-xl text-gray-600 leading-relaxed">{article.fullContent}</p>
                </div>

                <Card className="bg-white shadow-sm border border-gray-200 overflow-hidden mb-8">
                  <img 
                    src={article.image}
                    alt={`Illustratie bij artikel over ${article.id}`}
                    className="w-full h-64 md:h-80 object-cover"
                  />
                </Card>

                <div className="prose prose-lg max-w-none">
                  <div className={`${getImpactClasses(article.impactType)} p-6 mb-8 rounded-r-lg`}>
                    <h3 className={`text-lg font-semibold mb-2 ${article.impactType === 'positive' ? 'text-green-800' : article.impactType === 'warning' ? 'text-orange-800' : 'text-gray-800'}`}>
                      {article.impactType === 'positive' ? '📊' : article.impactType === 'warning' ? '⚠️' : '🏘️'} Impact op sociale ongelijkheid
                    </h3>
                    <p className={`mb-0 ${article.impactType === 'positive' ? 'text-green-700' : article.impactType === 'warning' ? 'text-orange-700' : 'text-gray-700'}`}>
                      <strong>Status:</strong> {article.impact}
                    </p>
                  </div>

                  <Card className="bg-white shadow-sm border border-gray-200 p-6 md:p-8">
                    <h3 className="text-xl font-semibold text-gray-900 mb-4">Politieke reacties</h3>
                    <div className="space-y-4">
                      {article.reactions.map((reaction, index) => (
                        <div key={index} className="flex items-start space-x-3">
                          <div className="w-6 h-6 bg-gray-100 rounded-full flex items-center justify-center text-sm">
                            {reaction.icon}
                          </div>
                          <div>
                            <p className="font-medium text-gray-900">{reaction.party}: {reaction.sentiment}</p>
                            <p className="text-gray-600 text-sm">{reaction.description}</p>
                          </div>
                        </div>
                      ))}
                    </div>
                  </Card>
                </div>
              </div>
            </article>
          )
        ))}

      </main>

      {/* Footer */}
      <footer className="bg-gray-900 text-white py-12 mt-16">
        <div className="max-w-6xl mx-auto px-4">
          <div className="text-center">
            <h3 className="text-xl font-semibold mb-4">📰 Het Nieuws in 2040</h3>
            <p className="text-gray-400 mb-6">Een blik op de toekomst van Nederland</p>
            <div className="border-t border-gray-700 pt-6">
              <p className="text-sm text-gray-500">
                &copy; 2040 Toekomstredactie – Gemaakt voor de praktische opdracht maatschappijleer.
              </p>
            </div>
          </div>
        </div>
      </footer>
    </div>
  );
}
