<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pedro Ambrósio Benko - Neuropsicologia</title>
    
    <!-- Carregar Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Carregar React e ReactDOM -->
    <script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    
    <!-- Carregar Babel para traduzir o código React no navegador -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

    <!-- Google Fonts (Opcional, para ficar mais bonito) -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>
        body { font-family: 'Inter', sans-serif; }
        
        /* Animações personalizadas */
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .animate-fade-in-up {
            animation: fadeInUp 0.8s ease-out forwards;
        }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        const { useState, useEffect } = React;

        // --- ÍCONES (Recriados aqui para não precisar de importação externa complexa) ---
        const Icon = ({ children, className }) => (
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round" className={className}>
                {children}
            </svg>
        );

        const Menu = ({ className }) => <Icon className={className}><line x1="4" x2="20" y1="12" y2="12"/><line x1="4" x2="20" y1="6" y2="6"/><line x1="4" x2="20" y1="18" y2="18"/></Icon>;
        const X = ({ className }) => <Icon className={className}><path d="M18 6 6 18"/><path d="m6 6 12 12"/></Icon>;
        const Phone = ({ className }) => <Icon className={className}><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></Icon>;
        const MapPin = ({ className }) => <Icon className={className}><path d="M20 10c0 6-8 12-8 12s-8-6-8-12a8 8 0 0 1 16 0Z"/><circle cx="12" cy="10" r="3"/></Icon>;
        const Mail = ({ className }) => <Icon className={className}><rect width="20" height="16" x="2" y="4" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></Icon>;
        const Brain = ({ className }) => <Icon className={className}><path d="M9.5 2A2.5 2.5 0 0 1 12 4.5v15a2.5 2.5 0 0 1-4.96.44 2.5 2.5 0 0 1-2.96-3.08 3 3 0 0 1-.34-5.58 2.5 2.5 0 0 1 1.32-4.24 2.5 2.5 0 0 1 1.98-3A2.5 2.5 0 0 1 9.5 2Z"/><path d="M14.5 2A2.5 2.5 0 0 0 12 4.5v15a2.5 2.5 0 0 0 4.96.44 2.5 2.5 0 0 0 2.96-3.08 3 3 0 0 0 .34-5.58 2.5 2.5 0 0 0-1.32-4.24 2.5 2.5 0 0 0-1.98-3A2.5 2.5 0 0 0 14.5 2Z"/></Icon>;
        const Activity = ({ className }) => <Icon className={className}><path d="M22 12h-4l-3 9L9 3l-3 9H2"/></Icon>;
        const FileText = ({ className }) => <Icon className={className}><path d="M14.5 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7.5L14.5 2z"/><polyline points="14 2 14 8 20 8"/><line x1="16" x2="8" y1="13" y2="13"/><line x1="16" x2="8" y1="17" y2="17"/><line x1="10" x2="8" y1="9" y2="9"/></Icon>;
        const ArrowRight = ({ className }) => <Icon className={className}><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></Icon>;
        const MessageCircle = ({ className }) => <Icon className={className}><path d="m3 21 1.9-5.7a8.5 8.5 0 1 1 3.8 3.8z"/></Icon>;
        const CheckCircle = ({ className }) => <Icon className={className}><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></Icon>;
        const Puzzle = ({ className }) => <Icon className={className}><path d="M19.439 7.85c0 .049.001.098.001.15a2 2 0 0 1-2 2h-1.5a2 2 0 0 0-2 2v1.5a2 2 0 0 1-4 0v-1.5a2 2 0 0 0-2-2h-1.5a2 2 0 0 1-2-2c0-.052 0-.101.001-.15a4.5 4.5 0 0 1 8.999 0Z"/><path d="M21 16h-1.5a2 2 0 0 0-2 2v1.5a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-1.5a2 2 0 0 0-2-2H8"/><path d="M4.561 16.15c0-.049-.001-.098-.001-.15a2 2 0 0 1 2-2h1.5a2 2 0 0 0 2-2v-1.5a2 2 0 0 1 4 0v1.5a2 2 0 0 0 2 2h1.5a2 2 0 0 1 2 2c0 .052 0 .101-.001.15a4.5 4.5 0 0 1-8.999 0Z"/></Icon>;
        const Instagram = ({ className }) => <Icon className={className}><rect width="20" height="20" x="2" y="2" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"/></Icon>;

        const Website = () => {
          const [isMenuOpen, setIsMenuOpen] = useState(false);
          const [currentPage, setCurrentPage] = useState('home');
          const [showScrollTop, setShowScrollTop] = useState(false);

          const professionalData = {
            name: "Pedro Ambrósio Benko",
            crp: "08/46329",
            specialty: "Neuropsicologia & Terapia Cognitivo-Comportamental",
            phone: "(41) 99902-5165",
            email: "contato.benko@gmail.com",
            address: "Atendimento Online para todo o Brasil",
            whatsappLink: "https://wa.me/5541999025165",
            instagram: "@neuropedroambrosio"
          };

          useEffect(() => {
            const handleScroll = () => {
              setShowScrollTop(window.scrollY > 300);
            };
            window.addEventListener('scroll', handleScroll);
            return () => window.removeEventListener('scroll', handleScroll);
          }, []);

          const navigateTo = (page) => {
            setCurrentPage(page);
            setIsMenuOpen(false);
            window.scrollTo(0, 0);
          };

          const Header = () => (
            <header className="bg-white shadow-sm fixed w-full top-0 z-50">
              <div className="container mx-auto px-4 sm:px-6 lg:px-8">
                <div className="flex justify-between items-center h-20">
                  <div className="flex items-center cursor-pointer" onClick={() => navigateTo('home')}>
                    <div className="bg-indigo-50 p-2 rounded-lg mr-3">
                      <Brain className="h-6 w-6 text-indigo-700" />
                    </div>
                    <div>
                      <h1 className="text-xl font-bold text-slate-800">{professionalData.name}</h1>
                      <p className="text-xs text-indigo-600 font-bold tracking-wide">NEUROPSICOLOGIA</p>
                    </div>
                  </div>
                  
                  <nav className="hidden md:flex space-x-8">
                    {['Início', 'Sobre', 'Avaliação', 'Terapia', 'Contato'].map((item) => {
                      const pageSlug = item.toLowerCase().replace('í', 'i').replace('ç', 'c').replace('ã', 'a');
                      return (
                        <button
                          key={item}
                          onClick={() => navigateTo(pageSlug === 'inicio' ? 'home' : pageSlug)}
                          className={`text-sm font-medium transition-colors ${
                            currentPage === (pageSlug === 'inicio' ? 'home' : pageSlug) 
                            ? 'text-indigo-600 border-b-2 border-indigo-600' 
                            : 'text-slate-500 hover:text-indigo-600'
                          }`}
                        >
                          {item}
                        </button>
                      );
                    })}
                    <a 
                      href={professionalData.whatsappLink}
                      target="_blank"
                      rel="noopener noreferrer"
                      className="bg-indigo-600 text-white px-5 py-2 rounded-full text-sm font-medium hover:bg-indigo-700 transition-colors shadow-md shadow-indigo-200"
                    >
                      Agendar
                    </a>
                  </nav>

                  <div className="md:hidden">
                    <button onClick={() => setIsMenuOpen(!isMenuOpen)} className="text-slate-500 hover:text-indigo-700">
                      {isMenuOpen ? <X className="h-6 w-6" /> : <Menu className="h-6 w-6" />}
                    </button>
                  </div>
                </div>
              </div>

              {isMenuOpen && (
                <div className="md:hidden bg-white border-t border-slate-100">
                  <div className="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                    {['Início', 'Sobre', 'Avaliação', 'Terapia', 'Contato'].map((item) => {
                      const pageSlug = item.toLowerCase().replace('í', 'i').replace('ç', 'c').replace('ã', 'a');
                      return (
                        <button
                          key={item}
                          onClick={() => navigateTo(pageSlug === 'inicio' ? 'home' : pageSlug)}
                          className="block w-full text-left px-3 py-2 rounded-md text-base font-medium text-slate-700 hover:text-indigo-600 hover:bg-indigo-50"
                        >
                          {item}
                        </button>
                      );
                    })}
                  </div>
                </div>
              )}
            </header>
          );

          const Footer = () => (
            <footer className="bg-slate-900 text-slate-300 pt-16 pb-8 border-t-4 border-indigo-500">
              <div className="container mx-auto px-4">
                <div className="grid grid-cols-1 md:grid-cols-3 gap-12 mb-12">
                  <div>
                    <div className="flex items-center mb-6">
                      <Brain className="h-8 w-8 text-indigo-400 mr-2" />
                      <div>
                        <h3 className="text-xl font-bold text-white">{professionalData.name}</h3>
                        <p className="text-xs text-indigo-400 uppercase tracking-widest">Neuropsicologia Clínica</p>
                      </div>
                    </div>
                    <p className="text-sm leading-relaxed mb-6 opacity-80">
                      Dedicação à compreensão das funções cognitivas e do comportamento humano. Unindo a ciência do cérebro com o acolhimento da psicologia.
                    </p>
                    <div className="flex gap-4">
                      <a href={`mailto:${professionalData.email}`} className="w-8 h-8 rounded bg-slate-800 flex items-center justify-center hover:bg-indigo-600 transition cursor-pointer">
                         <Mail className="h-4 w-4" />
                      </a>
                      <a href={professionalData.whatsappLink} target="_blank" rel="noopener noreferrer" className="w-8 h-8 rounded bg-slate-800 flex items-center justify-center hover:bg-green-600 transition cursor-pointer">
                         <MessageCircle className="h-4 w-4" />
                      </a>
                      <a href={`https://instagram.com/${professionalData.instagram.replace('@', '')}`} target="_blank" rel="noopener noreferrer" className="w-8 h-8 rounded bg-slate-800 flex items-center justify-center hover:bg-pink-600 transition cursor-pointer">
                         <Instagram className="h-4 w-4" />
                      </a>
                    </div>
                  </div>
                  
                  <div>
                    <h4 className="text-lg font-bold text-white mb-6">Especialidades</h4>
                    <ul className="space-y-3 text-sm">
                      <li className="flex items-center"><ArrowRight className="h-3 w-3 text-indigo-500 mr-2" /> Avaliação Neuropsicológica</li>
                      <li className="flex items-center"><ArrowRight className="h-3 w-3 text-indigo-500 mr-2" /> Terapia Cognitivo-Comportamental</li>
                      <li className="flex items-center"><ArrowRight className="h-3 w-3 text-indigo-500 mr-2" /> Reabilitação Cognitiva</li>
                      <li className="flex items-center"><ArrowRight className="h-3 w-3 text-indigo-500 mr-2" /> TDAH e Transtornos de Aprendizagem</li>
                      <li className="flex items-center"><ArrowRight className="h-3 w-3 text-indigo-500 mr-2" /> Avaliação de Idosos (Demências)</li>
                    </ul>
                  </div>

                  <div>
                    <h4 className="text-lg font-bold text-white mb-6">Localização</h4>
                    <ul className="space-y-4 text-sm">
                      <li className="flex items-start">
                        <MapPin className="h-5 w-5 text-indigo-500 mr-3 mt-1" />
                        <span>{professionalData.address}</span>
                      </li>
                      <li className="flex items-center">
                        <Phone className="h-5 w-5 text-indigo-500 mr-3" />
                        <span>{professionalData.phone}</span>
                      </li>
                      <li className="flex items-center">
                        <Mail className="h-5 w-5 text-indigo-500 mr-3" />
                        <span>{professionalData.email}</span>
                      </li>
                      <li className="flex items-center">
                        <Instagram className="h-5 w-5 text-indigo-500 mr-3" />
                        <span>{professionalData.instagram}</span>
                      </li>
                    </ul>
                  </div>
                </div>
                
                <div className="border-t border-slate-800 pt-8 text-center text-xs text-slate-500">
                  <p>&copy; {new Date().getFullYear()} {professionalData.name} - CRP {professionalData.crp}. Todos os direitos reservados.</p>
                  <p className="mt-2">Este site segue as diretrizes do Conselho Federal de Psicologia.</p>
                </div>
              </div>
            </footer>
          );

          const HomePage = () => (
            <div className="pt-20">
              <section className="relative bg-gradient-to-br from-white via-indigo-50/30 to-slate-50 py-24 lg:py-32 overflow-hidden">
                <div className="absolute top-0 right-0 w-1/3 h-full bg-indigo-50/50 skew-x-12 transform origin-top-right z-0"></div>
                
                <div className="container mx-auto px-4 relative z-10">
                  <div className="grid md:grid-cols-2 gap-16 items-center">
                    <div className="space-y-8 animate-fade-in-up">
                      <div className="inline-flex items-center space-x-2 bg-white border border-indigo-100 rounded-full px-4 py-1 shadow-sm">
                        <span className="w-2 h-2 rounded-full bg-indigo-600 animate-pulse"></span>
                        <span className="text-xs font-bold text-indigo-900 uppercase tracking-wide">Neurociência & Comportamento</span>
                      </div>
                      
                      <h1 className="text-4xl lg:text-5xl font-extrabold text-slate-900 leading-tight">
                        Entenda como seu cérebro <span className="text-indigo-600">funciona</span> para viver melhor.
                      </h1>
                      
                      <p className="text-lg text-slate-600 leading-relaxed max-w-lg">
                        Atendimento especializado em <strong>Avaliação Neuropsicológica</strong> e <strong>TCC</strong>. Investigamos a relação entre funções cognitivas, emoções e comportamento para promover diagnósticos precisos e tratamentos eficazes.
                      </p>
                      
                      <div className="flex flex-col sm:flex-row gap-4 pt-4">
                        <button onClick={() => navigateTo('avaliacao')} className="bg-indigo-600 text-white px-8 py-4 rounded-xl font-bold hover:bg-indigo-700 transition shadow-lg shadow-indigo-600/20 flex items-center justify-center">
                          Avaliação Neuropsicológica
                        </button>
                        <button onClick={() => navigateTo('terapia')} className="bg-white text-slate-700 border border-slate-200 px-8 py-4 rounded-xl font-bold hover:bg-slate-50 transition flex items-center justify-center">
                          Conhecer a TCC
                        </button>
                      </div>
                    </div>

                    <div className="relative">
                      <div className="grid grid-cols-2 gap-4">
                        <div className="space-y-4 translate-y-8">
                          <div className="bg-white p-4 rounded-2xl shadow-lg border border-indigo-50">
                            <Brain className="h-8 w-8 text-indigo-600 mb-2" />
                            <p className="text-xs font-bold text-slate-800">Cognição</p>
                            <p className="text-[10px] text-slate-500">Memória & Atenção</p>
                          </div>
                          <img src="https://images.unsplash.com/photo-1559757175-5700dde675bc?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" className="rounded-2xl shadow-lg object-cover h-48 w-full" alt="Materiais de teste" />
                        </div>
                        <div className="space-y-4">
                          <img src="https://images.unsplash.com/photo-1576091160399-112ba8d25d1d?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" className="rounded-2xl shadow-lg object-cover h-48 w-full" alt="Cérebro digital" />
                          <div className="bg-indigo-600 p-4 rounded-2xl shadow-lg text-white">
                            <Activity className="h-8 w-8 mb-2 text-indigo-200" />
                            <p className="text-xs font-bold">Diagnóstico</p>
                            <p className="text-[10px] text-indigo-200">Baseado em evidências</p>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </section>

              <section className="py-24 bg-white">
                <div className="container mx-auto px-4">
                  <div className="max-w-3xl mx-auto text-center mb-16">
                    <h2 className="text-3xl font-bold text-slate-900 mb-4">Uma abordagem integrativa</h2>
                    <p className="text-slate-600">
                      Unimos o rigor técnico da avaliação neuropsicológica com a eficácia prática da Terapia Cognitivo-Comportamental.
                    </p>
                  </div>

                  <div className="grid md:grid-cols-3 gap-8">
                    <div className="bg-slate-50 p-8 rounded-2xl border border-slate-100 hover:border-indigo-200 transition duration-300">
                      <div className="w-12 h-12 bg-indigo-100 rounded-lg flex items-center justify-center mb-6">
                        <FileText className="h-6 w-6 text-indigo-600" />
                      </div>
                      <h3 className="text-xl font-bold text-slate-900 mb-3">Avaliação Precisa</h3>
                      <p className="text-slate-600 text-sm leading-relaxed">
                        Uso de testes padronizados para investigar TDAH, Autismo, perdas de memória em idosos e outras alterações cognitivas.
                      </p>
                    </div>
                    
                    <div className="bg-slate-50 p-8 rounded-2xl border border-slate-100 hover:border-indigo-200 transition duration-300">
                      <div className="w-12 h-12 bg-blue-100 rounded-lg flex items-center justify-center mb-6">
                        <Puzzle className="h-6 w-6 text-blue-600" />
                      </div>
                      <h3 className="text-xl font-bold text-slate-900 mb-3">Reabilitação</h3>
                      <p className="text-slate-600 text-sm leading-relaxed">
                        Treino cognitivo para recuperar ou compensar funções como atenção, memória e planejamento que estejam prejudicadas.
                      </p>
                    </div>

                    <div className="bg-slate-50 p-8 rounded-2xl border border-slate-100 hover:border-indigo-200 transition duration-300">
                      <div className="w-12 h-12 bg-teal-100 rounded-lg flex items-center justify-center mb-6">
                        <MessageCircle className="h-6 w-6 text-teal-600" />
                      </div>
                      <h3 className="text-xl font-bold text-slate-900 mb-3">Terapia (TCC)</h3>
                      <p className="text-slate-600 text-sm leading-relaxed">
                        Foco na reestruturação de pensamentos e mudança de comportamentos para tratar ansiedade, depressão e fobias.
                      </p>
                    </div>
                  </div>
                </div>
              </section>

              <section className="bg-indigo-900 py-16">
                <div className="container mx-auto px-4 text-center">
                  <h2 className="text-2xl md:text-3xl font-bold text-white mb-6">Precisa de um laudo neuropsicológico ou acompanhamento?</h2>
                  <p className="text-indigo-200 mb-8 max-w-2xl mx-auto">
                    Atendimentos para crianças, adolescentes, adultos e idosos. Agende uma conversa inicial para entendermos sua demanda.
                  </p>
                  <button onClick={() => navigateTo('contato')} className="bg-white text-indigo-900 px-8 py-3 rounded-full font-bold hover:bg-indigo-50 transition">
                    Entrar em Contato
                  </button>
                </div>
              </section>
            </div>
          );

          const AboutPage = () => (
            <div className="pt-28 pb-20 bg-slate-50 min-h-screen">
              <div className="container mx-auto px-4">
                <div className="bg-white rounded-3xl overflow-hidden shadow-sm border border-slate-100">
                  <div className="grid md:grid-cols-2 gap-8 items-center p-8 md:p-12">
                    <div className="order-2 md:order-1 flex flex-col justify-center">
                      <span className="text-indigo-600 font-bold tracking-wider text-xs uppercase mb-2">PÓS GRADUANDO EM NEUROPSICOLOGIA</span>
                      <h1 className="text-3xl md:text-4xl font-bold text-slate-900 mb-6">{professionalData.name}</h1>
                      
                      <div className="space-y-4 text-slate-600 leading-relaxed mb-8">
                        <p>
                          Olá! Sou Pedro Ambrosio Benko, psicólogo formado pela Unibrasil e pós-graduando em Neuropsicologia pela FAE.
                        </p>
                        <p>
                          Tenho experiência em atendimento clínico, atuando com crianças, adolescentes, adultos e idosos sempre com foco em oferecer uma escuta acolhedora, responsável e baseada em evidências.
                        </p>
                        <p>
                          Na clínica, utilizo a <strong>Terapia Cognitivo-Comportamental (TCC)</strong>, uma abordagem estruturada e diretiva. Acredito que o consultório deve ser um espaço seguro, livre de julgamentos, onde trabalhamos juntos para identificar padrões e promover mudanças positivas.
                        </p>
                      </div>

                      <div className="grid grid-cols-1 sm:grid-cols-2 gap-4">
                        <div className="flex items-center text-sm text-slate-700 bg-slate-50 p-3 rounded-lg">
                          <CheckCircle className="h-5 w-5 text-indigo-500 mr-2" /> Exp. em Reabilitação Neuropsicológica
                        </div>
                        <div className="flex items-center text-sm text-slate-700 bg-slate-50 p-3 rounded-lg">
                          <CheckCircle className="h-5 w-5 text-indigo-500 mr-2" /> Crianças e Adolescentes
                        </div>
                        <div className="flex items-center text-sm text-slate-700 bg-slate-50 p-3 rounded-lg">
                          <CheckCircle className="h-5 w-5 text-indigo-500 mr-2" /> Adultos e Idosos
                        </div>
                        <div className="flex items-center text-sm text-slate-700 bg-slate-50 p-3 rounded-lg">
                          <CheckCircle className="h-5 w-5 text-indigo-500 mr-2" /> CRP: {professionalData.crp}
                        </div>
                      </div>
                    </div>
                    
                    <div className="order-1 md:order-2 flex justify-center items-center">
                       <div className="relative">
                         <div className="absolute inset-0 bg-indigo-200 rounded-full blur-2xl opacity-40 transform scale-110"></div>
                         
                         <div className="w-64 h-64 relative rounded-full border-4 border-white shadow-xl overflow-hidden">
                            {/* IMPORTANTE: Aqui é onde você troca pela sua foto local se desejar. */}
                            <img 
                              src="./pb.jpg" 
                              className="w-full h-full object-cover" 
                              alt="Pedro Ambrósio Benko" 
                            />
                         </div>
                       </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          );

          const AvaliacaoPage = () => (
            <div className="pt-28 pb-20 bg-slate-50 min-h-screen">
              <div className="container mx-auto px-4">
                <div className="max-w-3xl mx-auto mb-12 text-center">
                  <div className="inline-block p-3 bg-indigo-100 rounded-full mb-4">
                    <FileText className="h-8 w-8 text-indigo-600" />
                  </div>
                  <h1 className="text-3xl md:text-4xl font-bold text-slate-900 mb-4">Avaliação Neuropsicológica</h1>
                  <p className="text-slate-600 text-lg">Um mapeamento detalhado das funções cognitivas.</p>
                </div>

                <div className="bg-white rounded-2xl shadow-sm border border-slate-100 p-8 md:p-12 mb-12">
                  <h3 className="text-xl font-bold text-slate-900 mb-6">O que é e para que serve?</h3>
                  <div className="prose text-slate-600 max-w-none space-y-4">
                    <p>
                      A avaliação neuropsicológica é um exame complementar que investiga o funcionamento do cérebro através de testes, escalas e entrevistas. Ela é fundamental para auxiliar médicos (neurologistas e psiquiatras) no diagnóstico diferencial.
                    </p>
                    <p><strong>Avaliamos funções como:</strong> Atenção, memória, linguagem, raciocínio lógico, planejamento (funções executivas) e humor.</p>
                  </div>
                  
                  <div className="grid md:grid-cols-2 gap-6 mt-8">
                    <div className="bg-indigo-50 p-6 rounded-xl border border-indigo-100">
                      <h4 className="font-bold text-indigo-900 mb-2">Público Infantojuvenil</h4>
                      <ul className="text-sm text-indigo-800 space-y-2">
                        <li>• Suspeita de TDAH (Déficit de Atenção)</li>
                        <li>• Transtorno do Espectro Autista (TEA)</li>
                        <li>• Dificuldades de aprendizagem e Dislexia</li>
                        <li>• Atrasos no desenvolvimento</li>
                      </ul>
                    </div>
                    <div className="bg-blue-50 p-6 rounded-xl border border-blue-100">
                      <h4 className="font-bold text-blue-900 mb-2">Adultos e Idosos</h4>
                      <ul className="text-sm text-blue-800 space-y-2">
                        <li>• Queixas de memória (Alzheimer e demências)</li>
                        <li>• Sequelas pós-AVC ou TCE</li>
                        <li>• Diagnóstico diferencial de depressão x demência</li>
                        <li>• Avaliação de capacidade cognitiva</li>
                      </ul>
                    </div>
                  </div>
                </div>

                <div className="bg-slate-900 text-white rounded-2xl p-8 md:p-12 flex flex-col md:flex-row items-center justify-between gap-8">
                  <div>
                    <h3 className="text-xl font-bold mb-2">Como funciona o processo?</h3>
                    <p className="text-slate-300 text-sm">Geralmente são necessárias de 10 a 12 sessões para aplicação dos testes, finalizando com uma sessão de devolutiva e entrega do laudo técnico.</p>
                  </div>
                  <button onClick={() => navigateTo('contato')} className="bg-indigo-500 hover:bg-indigo-600 text-white px-6 py-3 rounded-lg font-bold transition whitespace-nowrap">
                    Solicitar Orçamento
                  </button>
                </div>
              </div>
            </div>
          );

          const TerapiaPage = () => (
            <div className="pt-28 pb-20 bg-slate-50 min-h-screen">
              <div className="container mx-auto px-4">
                <div className="grid md:grid-cols-2 gap-12 items-start">
                  <div>
                    <span className="text-indigo-600 font-bold tracking-wider text-xs uppercase mb-2">Psicoterapia</span>
                    <h1 className="text-3xl md:text-4xl font-bold text-slate-900 mb-6">Terapia Cognitivo-Comportamental (TCC)</h1>
                    <div className="prose text-slate-600 space-y-4 leading-relaxed">
                      <p>
                        A TCC é uma abordagem estruturada, colaborativa e focada no presente. A premissa central é que não são os eventos em si que nos afetam, mas sim a <strong>forma como interpretamos</strong> esses eventos.
                      </p>
                      <p>
                        Nas sessões, trabalhamos para identificar pensamentos disfuncionais (distorções cognitivas) que geram sofrimento e comportamentos que perpetuam o problema.
                      </p>
                      <p>
                        É o tratamento de primeira escolha para quadros de ansiedade, pânico, depressão e TOC, com robustas evidências científicas de eficácia.
                      </p>
                    </div>

                    <div className="mt-8 grid gap-4">
                      <div className="bg-white p-4 rounded-lg shadow-sm border border-slate-100 flex items-start">
                        <Brain className="h-6 w-6 text-indigo-600 mr-4 mt-1" />
                        <div>
                          <h4 className="font-bold text-slate-800">Reabilitação Cognitiva</h4>
                          <p className="text-sm text-slate-500 mt-1">
                            Além da terapia, ofereço sessões focadas em exercícios para estimular o cérebro, ideal para idosos com declínio cognitivo ou pacientes pós-lesão.
                          </p>
                        </div>
                      </div>
                    </div>
                  </div>

                  <div className="bg-white p-8 rounded-2xl shadow-lg border border-slate-100">
                    <h3 className="text-xl font-bold text-slate-900 mb-6">Áreas de Atuação</h3>
                    <div className="space-y-4">
                      {[
                        "Transtornos de Ansiedade (TAG, Pânico, Fobias)",
                        "Depressão e Transtornos de Humor",
                        "Transtorno de Déficit de Atenção (TDAH)",
                        "Treino de Habilidades Sociais",
                        "Gestão do Estresse e Burnout",
                        "Estimulação Cognitiva para Idosos"
                      ].map((item, idx) => (
                        <div key={idx} className="flex items-center p-3 hover:bg-slate-50 rounded-lg transition border border-transparent hover:border-slate-100">
                          <div className="h-2 w-2 bg-indigo-500 rounded-full mr-3"></div>
                          <span className="text-slate-700 font-medium">{item}</span>
                        </div>
                      ))}
                    </div>
                    <div className="mt-8 pt-6 border-t border-slate-100">
                      <p className="text-sm text-slate-500 mb-4">
                        Atendimentos presenciais e online (autorizado pelo E-Psi).
                      </p>
                      <button onClick={() => navigateTo('contato')} className="w-full bg-slate-800 text-white py-3 rounded-lg font-bold hover:bg-slate-900 transition">
                        Agendar Terapia
                      </button>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          );

          const ContactPage = () => (
            <div className="pt-28 pb-20 bg-slate-50 min-h-screen">
              <div className="container mx-auto px-4">
                <div className="grid md:grid-cols-2 gap-12">
                  <div>
                    <h1 className="text-3xl font-bold text-slate-900 mb-6">Agendamento & Contato</h1>
                    <p className="text-slate-600 mb-8">
                      Entre em contato para verificar disponibilidade para <strong>Avaliação Neuropsicológica</strong> ou <strong>Psicoterapia</strong>.
                    </p>

                    <div className="space-y-6">
                      <div className="flex items-start bg-white p-6 rounded-xl shadow-sm border border-slate-100 hover:shadow-md transition">
                        <div className="bg-green-100 p-3 rounded-lg mr-4">
                          <MessageCircle className="h-6 w-6 text-green-600" />
                        </div>
                        <div>
                          <h3 className="font-bold text-slate-800">WhatsApp Profissional</h3>
                          <p className="text-sm text-slate-500 mb-2">Resposta rápida para agendamentos.</p>
                          <a href={professionalData.whatsappLink} target="_blank" rel="noopener noreferrer" className="text-green-600 font-bold hover:underline text-sm flex items-center">
                            Iniciar conversa <ArrowRight className="h-4 w-4 ml-1" />
                          </a>
                        </div>
                      </div>

                      <div className="flex items-start bg-white p-6 rounded-xl shadow-sm border border-slate-100 hover:shadow-md transition">
                        <div className="bg-pink-100 p-3 rounded-lg mr-4">
                          <Instagram className="h-6 w-6 text-pink-600" />
                        </div>
                        <div>
                          <h3 className="font-bold text-slate-800">Instagram</h3>
                          <p className="text-sm text-slate-500 mb-1">Acompanhe conteúdos exclusivos.</p>
                          <a href={`https://instagram.com/${professionalData.instagram.replace('@', '')}`} target="_blank" rel="noopener noreferrer" className="text-pink-600 font-bold hover:underline text-sm">
                            {professionalData.instagram}
                          </a>
                        </div>
                      </div>

                      <div className="flex items-start bg-white p-6 rounded-xl shadow-sm border border-slate-100 hover:shadow-md transition">
                        <div className="bg-indigo-100 p-3 rounded-lg mr-4">
                          <Mail className="h-6 w-6 text-indigo-600" />
                        </div>
                        <div>
                          <h3 className="font-bold text-slate-800">E-mail</h3>
                          <p className="text-sm text-slate-500">{professionalData.email}</p>
                        </div>
                      </div>

                      <div className="flex items-start bg-white p-6 rounded-xl shadow-sm border border-slate-100 hover:shadow-md transition">
                        <div className="bg-blue-100 p-3 rounded-lg mr-4">
                          <MapPin className="h-6 w-6 text-blue-600" />
                        </div>
                        <div>
                          <h3 className="font-bold text-slate-800">Atendimento</h3>
                          <p className="text-sm text-slate-500">{professionalData.address}</p>
                          <p className="text-xs text-slate-400 mt-1">Sessões via videochamada segura.</p>
                        </div>
                      </div>
                    </div>
                  </div>

                  <div className="bg-white p-8 rounded-2xl shadow-lg border border-slate-100 relative overflow-hidden">
                    <div className="absolute top-0 right-0 w-20 h-20 bg-indigo-100 rounded-bl-full -mr-10 -mt-10"></div>
                    <h3 className="text-xl font-bold text-slate-800 mb-6 relative z-10">Envie sua mensagem</h3>
                    <form className="space-y-4 relative z-10" onSubmit={(e) => e.preventDefault()}>
                      <div>
                        <label className="block text-sm font-bold text-slate-700 mb-1">Nome Completo</label>
                        <input type="text" className="w-full px-4 py-3 border border-slate-200 bg-slate-50 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition" placeholder="Seu nome" />
                      </div>
                      
                      <div className="grid grid-cols-2 gap-4">
                        <div>
                          <label className="block text-sm font-bold text-slate-700 mb-1">Telefone</label>
                          <input type="tel" className="w-full px-4 py-3 border border-slate-200 bg-slate-50 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition" placeholder="(DDD)" />
                        </div>
                        <div>
                          <label className="block text-sm font-bold text-slate-700 mb-1">Motivo</label>
                           <select className="w-full px-4 py-3 border border-slate-200 bg-slate-50 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition text-slate-600">
                             <option>Terapia (TCC)</option>
                             <option>Avaliação Neuropsicológica</option>
                             <option>Reabilitação Cognitiva</option>
                             <option>Outros</option>
                           </select>
                        </div>
                      </div>

                      <div>
                        <label className="block text-sm font-bold text-slate-700 mb-1">Mensagem</label>
                        <textarea rows="4" className="w-full px-4 py-3 border border-slate-200 bg-slate-50 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent outline-none transition" placeholder="Breve relato sobre sua busca..." />
                      </div>

                      <button className="w-full bg-indigo-600 text-white py-4 rounded-lg font-bold hover:bg-indigo-700 transition shadow-lg shadow-indigo-600/20">
                        Enviar Solicitação
                      </button>
                    </form>
                  </div>
                </div>
              </div>
            </div>
          );

          return (
            <div className="min-h-screen bg-white font-sans text-slate-900">
              <Header />
              <main>
                {currentPage === 'home' && <HomePage />}
                {currentPage === 'sobre' && <AboutPage />}
                {currentPage === 'avaliacao' && <AvaliacaoPage />}
                {currentPage === 'terapia' && <TerapiaPage />}
                {currentPage === 'contato' && <ContactPage />}
              </main>
              <Footer />
              
              <a 
                href={professionalData.whatsappLink}
                target="_blank"
                rel="noopener noreferrer"
                className="fixed bottom-6 right-6 bg-green-500 hover:bg-green-600 text-white p-4 rounded-full shadow-2xl transition-transform hover:scale-110 z-50 flex items-center justify-center group"
                aria-label="Contato via WhatsApp"
              >
                <span className="absolute right-full mr-3 bg-slate-800 text-white text-xs px-2 py-1 rounded opacity-0 group-hover:opacity-100 transition whitespace-nowrap">Agende agora</span>
                <MessageCircle className="h-8 w-8" />
              </a>

              {showScrollTop && (
                <button 
                  onClick={() => window.scrollTo({ top: 0, behavior: 'smooth' })}
                  className="fixed bottom-24 right-8 bg-slate-800/80 hover:bg-slate-900 text-white p-2 rounded-full shadow-lg transition z-40"
                >
                  <ArrowRight className="h-4 w-4 -rotate-90" />
                </button>
              )}
            </div>
          );
        };

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<Website />);
    </script>
</body>
</html>
