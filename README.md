<!DOCTYPE html>
<html lang="de" class="h-full">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DEPARTD · Testaufgabe Processes & Automation Architect</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Syne:wght@700;800&family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            neon: '#E4FF00',
                            darkBg: '#050508',
                            darkCard: '#0E0E16',
                            border: '#1F1F2E',
                            textMuted: '#94A3B8',
                        }
                    },
                    fontFamily: {
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                        syne: ['"Syne"', 'sans-serif'],
                        mono: ['"JetBrains Mono"', 'monospace'],
                    }
                }
            }
        }
    </script>
    
    <style>
        .neon-glow {
            box-shadow: 0 0 30px rgba(228, 255, 0, 0.15);
        }
        .neon-border-focus:focus {
            outline: none;
            border-color: #E4FF00;
            box-shadow: 0 0 15px rgba(228, 255, 0, 0.25);
        }
        .neon-text-glow {
            text-shadow: 0 0 15px rgba(228, 255, 0, 0.3);
        }
        .grid-bg {
            background-image: radial-gradient(rgba(228, 255, 0, 0.04) 1px, transparent 1px);
            background-size: 24px 24px;
        }
        @keyframes gradient-flow {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .animate-gradient {
            background-size: 200% auto;
            animation: gradient-flow 6s linear infinite;
        }
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
            height: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #050508;
        }
        ::-webkit-scrollbar-thumb {
            background: #1F1F2E;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #E4FF00;
        }
    </style>
</head>
<body class="bg-brand-darkBg text-white font-sans min-h-full flex flex-col justify-between overflow-x-hidden grid-bg">

    <!-- Top Decorative Gradient Bar -->
    <div class="h-1.5 w-full bg-gradient-to-r from-brand-neon via-cyan-400 to-purple-600 animate-gradient"></div>

    <header class="sticky top-0 px-6 py-4 md:px-12 flex flex-col md:flex-row justify-between items-center z-50 backdrop-blur-md bg-brand-darkBg/80 border-b border-brand-border/40 gap-4">
        <div class="flex items-center space-x-3">
            <div class="w-10 h-10 rounded-xl bg-brand-neon flex items-center justify-center font-extrabold text-black font-syne text-lg transform hover:rotate-6 transition-transform">D</div>
            <div class="flex flex-col">
                <span class="font-extrabold tracking-wider text-base font-syne">DEPARTD</span>
                <span class="text-xs text-brand-neon tracking-widest font-mono uppercase">Process Engine // Workspace</span>
            </div>
        </div>
        
        <!-- Minimalist Status Badge -->
        <div class="flex items-center space-x-3">
            <span class="bg-[#0E0E16] text-brand-textMuted px-4 py-2 rounded-full border border-brand-border/60 text-[10px] font-bold uppercase tracking-widest font-mono">
                TESTAUFGABE // CANDIDATE WORKSPACE
            </span>
        </div>
    </header>

    <main class="flex-grow max-w-6xl w-full mx-auto px-4 md:px-8 py-8 md:py-12 space-y-16">
        
        <!-- Hero Section with aligned Candidate Profile description -->
        <section class="space-y-6 text-center md:text-left relative">
            <div class="absolute -top-12 -left-12 w-48 h-48 bg-brand-neon/5 rounded-full blur-3xl pointer-events-none"></div>
            <div class="inline-flex items-center space-x-2 bg-brand-neon/10 border border-brand-neon/20 px-3 py-1.5 rounded-full text-brand-neon text-xs font-bold uppercase tracking-widest">
                <span class="w-2 h-2 rounded-full bg-brand-neon"></span>
                <span>Case Study: Werkstudent:in Processes & Automation (Process Architect)</span>
            </div>
            <h1 class="text-4xl md:text-6xl font-extrabold font-syne leading-tight">
                Baue die Brücken <br class="hidden md:block"/>
                unserer <span class="neon-text-glow text-brand-neon">Infrastruktur.</span>
            </h1>
            <p class="text-base md:text-lg text-brand-textMuted max-w-3xl leading-relaxed">
                Hi! Bei DEPARTD suchen wir keinen Kampagnen-Assistenten für das Tagesgeschäft. Wir suchen einen <strong>Infrastruktur-Kopf und Prozess-Architekten</strong>. Jemanden, der Datenflüsse automatisiert, Abteilungs-Silos (Creative, Finance, Operations) einreißt und die Agentur-Infrastruktur so lean und stabil baut, dass das operative Team ungestört skalieren kann. Zeig uns, wie dein Gehirn tickt!
            </p>
            
            <!-- Quick Facts Grid -->
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4 pt-6 max-w-4xl">
                <div class="bg-brand-darkCard border border-brand-border p-4 rounded-xl">
                    <div class="text-xs text-brand-textMuted font-mono">ZEITBUDGET</div>
                    <div class="text-base font-bold text-white mt-1">ca. 1–2 Stunden</div>
                </div>
                <div class="bg-brand-darkCard border border-brand-border p-4 rounded-xl">
                    <div class="text-xs text-brand-textMuted font-mono">PROFIL-FOKUS</div>
                    <div class="text-base font-bold text-white mt-1">Lean / Systems Architect</div>
                </div>
                <div class="bg-brand-darkCard border border-brand-border p-4 rounded-xl">
                    <div class="text-xs text-brand-textMuted font-mono">STEUERUNG</div>
                    <div class="text-base font-bold text-white mt-1">No-Code Hubs & APIs</div>
                </div>
                <div class="bg-brand-darkCard border border-brand-border p-4 rounded-xl">
                    <div class="text-xs text-brand-textMuted font-mono">EXPORT</div>
                    <div class="text-base font-bold text-brand-neon mt-1">1-Klick-Markdown</div>
                </div>
            </div>
        </section>

        <!-- Das DEPARTD Ökosystem -->
        <section class="bg-brand-darkCard border border-brand-border rounded-2xl p-6 md:p-8 relative overflow-hidden">
            <div class="absolute top-0 right-0 w-32 h-32 bg-purple-500/5 rounded-full blur-3xl pointer-events-none"></div>
            <div class="space-y-4">
                <div class="text-xs text-brand-neon font-mono uppercase tracking-widest">// 01 / DAS SYSTEM-ÖKOSYSTEM</div>
                <h2 class="text-2xl md:text-3xl font-extrabold font-syne">Unsere operativen Zahnräder</h2>
                <p class="text-sm text-brand-textMuted leading-relaxed max-w-3xl">
                    DEPARTD steuert hochfrequente Influencer-Kampagnen. Unser Herzstück ist die <strong>„Engine“</strong> – unsere hauseigene Software, in der alle Master-Daten zusammenlaufen. Damit die Daten fließen, verknüpfen wir verschiedene Systeme zu einer nahtlosen Schnittstellen-Infrastruktur:
                </p>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-4 pt-4">
                    <div class="bg-[#14141F]/60 p-4 rounded-xl border border-brand-border/40">
                        <div class="flex items-center space-x-2 text-brand-neon font-bold text-sm mb-2">
                            <span>M</span> <span>Monday.com</span>
                        </div>
                        <p class="text-xs text-brand-textMuted">Die operative Daten-Zentrale. Hier leben Workflows, Lead-Status und tagesaktuelle Kampagnen-Gigs.</p>
                    </div>
                    <div class="bg-[#14141F]/60 p-4 rounded-xl border border-brand-border/40">
                        <div class="flex items-center space-x-2 text-cyan-400 font-bold text-sm mb-2">
                            <span>N</span> <span>Notion API</span>
                        </div>
                        <p class="text-xs text-brand-textMuted">Unsere abteilungsübergreifende Wissens- und Content-Datenbank für Creative- und Sourcing-Teams.</p>
                    </div>
                    <div class="bg-[#14141F]/60 p-4 rounded-xl border border-brand-border/40">
                        <div class="flex items-center space-x-2 text-purple-400 font-bold text-sm mb-2">
                            <span>API</span> <span>No-Code & KI Hubs</span>
                        </div>
                        <p class="text-xs text-brand-textMuted">Z.B. Make oder n8n, gepaart mit OpenAI, um Daten über verschiedene Schnittstellen fehlerfrei zu synchronisieren.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Das Szenario: Die Ingest-Pipeline (Interaktives Flowchart) -->
        <section class="space-y-6">
            <div class="space-y-2">
                <div class="text-xs text-brand-neon font-mono uppercase tracking-widest">// 02 / DIE SCHNITTSTELLEN-ANALYSE</div>
                <h2 class="text-2xl md:text-3xl font-extrabold font-syne">Das Szenario: Daten-Ingestion-Pipeline</h2>
                <p class="text-sm text-brand-textMuted max-w-3xl leading-relaxed">
                    Daten über neue Creator und Kampagnen-Assets fließen täglich über unzählige Kanäle in unsere Systeme (Webformulare, Instagram-DMs, Scraper-Exporte, Team-Sourcing). Bevor die Daten für Teams nutzbar sind, müssen sie sauber prozessiert werden. 
                    <strong>Klicke auf die Schritte der aktuellen Pipeline, um die systemischen Reibungsverluste ("Silos") zu analysieren:</strong>
                </p>
            </div>

            <!-- Flowchart Simulator -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-6 items-stretch">
                <!-- Left Buttons -->
                <div class="lg:col-span-7 bg-brand-darkCard border border-brand-border rounded-2xl p-6 flex flex-col justify-between gap-4">
                    <span class="text-[10px] text-brand-textMuted uppercase font-mono tracking-wider block">Aktueller unstrukturierter Fluss (Klick für Details)</span>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-3">
                        <button onclick="selectFlowStep(1)" id="btn-flow-1" class="flow-btn active p-4 rounded-xl border border-brand-neon/40 bg-brand-neon/5 hover:bg-brand-neon/10 text-left transition-all duration-200">
                            <div class="step-badge text-[10px] font-bold text-brand-neon mb-1">SCHNITTSTELLE 1</div>
                            <div class="text-xs font-bold text-white">Datenquellen & Fragmentierung</div>
                            <div class="text-[9px] text-brand-textMuted mt-1">Multi-Channel Ingest ohne Vorvalidierung</div>
                        </button>
                        <button onclick="selectFlowStep(2)" id="btn-flow-2" class="flow-btn p-4 rounded-xl border border-brand-border bg-[#0E0E16]/30 hover:bg-brand-darkCard text-left transition-all duration-200">
                            <div class="step-badge text-[10px] font-bold text-brand-textMuted mb-1">SCHNITTSTELLE 2</div>
                            <div class="text-xs font-bold text-white">Daten-Inkonsistenz & Dubletten</div>
                            <div class="text-[9px] text-brand-textMuted mt-1">Mangelnder Dubletten-Check im Master-Board</div>
                        </button>
                        <button onclick="selectFlowStep(3)" id="btn-flow-3" class="flow-btn p-4 rounded-xl border border-brand-border bg-[#0E0E16]/30 hover:bg-brand-darkCard text-left transition-all duration-200">
                            <div class="step-badge text-[10px] font-bold text-brand-textMuted mb-1">SCHNITTSTELLE 3</div>
                            <div class="text-xs font-bold text-white">Unstrukturierter Medienbruch</div>
                            <div class="text-[9px] text-brand-textMuted mt-1">Screenshots & manuelles Datenabtippen</div>
                        </button>
                        <button onclick="selectFlowStep(4)" id="btn-flow-4" class="flow-btn p-4 rounded-xl border border-brand-border bg-[#0E0E16]/30 hover:bg-brand-darkCard text-left transition-all duration-200">
                            <div class="step-badge text-[10px] font-bold text-brand-textMuted mb-1">SCHNITTSTELLE 4</div>
                            <div class="text-xs font-bold text-white">Isolierte Kategorisierung (Silos)</div>
                            <div class="text-[9px] text-brand-textMuted mt-1">Subjektives Tagging blockiert Creative-Suchen</div>
                        </button>
                    </div>

                    <div class="p-3 bg-brand-darkBg/60 rounded-xl border border-brand-border/40 text-xs text-brand-textMuted flex items-center gap-2">
                        <span class="text-brand-neon font-mono">⚙️</span>
                        <span>Diese Infrastruktur-Herausforderungen bremsen das Skalieren aus. Behalte sie im Kopf für deine systemischen Lösungen gleich!</span>
                    </div>
                </div>

                <!-- Right Details (Dynamic) -->
                <div class="lg:col-span-5 bg-[#141421] border border-brand-border rounded-2xl p-6 flex flex-col justify-between" id="flow-details">
                    <div class="space-y-4">
                        <div class="flex justify-between items-center">
                            <span class="text-[10px] text-brand-neon uppercase font-mono tracking-widest font-bold">Systemische Schwachstelle</span>
                            <span class="px-2 py-0.5 rounded bg-red-500/15 text-red-400 text-[10px] font-bold tracking-widest uppercase" id="flow-risk">🔴 Hohe Reibung</span>
                        </div>
                        <h4 id="flow-title" class="text-xl font-bold text-white">Datenquellen & Fragmentierung</h4>
                        <p id="flow-desc" class="text-xs text-brand-textMuted leading-relaxed">
                            Daten strömen unstrukturiert über Webformulare, Mail-Postfächer und Direktnachrichten rein. Es existiert kein zentrales Gateway oder Ingest-Parser.
                        </p>
                        <div class="bg-red-500/10 border border-red-500/20 rounded-xl p-4 space-y-2">
                            <span class="text-[10px] font-bold uppercase tracking-widest text-red-400 block">Der systemische Verlust:</span>
                            <p id="flow-problem" class="text-[11px] text-red-300 leading-relaxed">
                                Strikte Daten-Silos. Operative Teams fischen Daten händisch aus Drittsystemen, anstatt dass diese strukturiert und vorvalidiert im Master-System eintreffen.
                            </p>
                        </div>
                    </div>
                    <div class="pt-4 border-t border-brand-border/40 flex justify-between items-center text-[10px] font-mono text-brand-textMuted">
                        <span>Workflow-Gattung: <strong class="text-red-400 uppercase" id="flow-clicks">Manuell & Dezentral</strong></span>
                    </div>
                </div>
            </div>
        </section>

        <!-- THE WORKSPACE WORKBOOK -->
        <section class="space-y-12 pt-8 border-t border-brand-border/60">
            <div class="text-center max-w-2xl mx-auto space-y-3">
                <div class="inline-flex items-center space-x-2 bg-brand-neon/15 px-3 py-1 rounded-full text-brand-neon text-xs font-bold font-mono uppercase tracking-wider">
                    <span>⚡ DEPARTD Live Workspace</span>
                </div>
                <h2 class="text-3xl md:text-4xl font-extrabold font-syne">Deine System-Entwürfe</h2>
                <p class="text-sm text-brand-textMuted">
                    Dokumentiere deine Konzepte direkt in den folgenden Modulen. Deine Daten werden lokal zwischengespeichert und können am Ende mit einem Klick exportiert werden.
                </p>
            </div>

            <!-- ================= TASK 1 ================= -->
            <div class="bg-brand-darkCard border border-brand-border rounded-2xl p-6 md:p-8 space-y-6">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b border-brand-border pb-4 gap-4">
                    <div>
                        <span class="text-xs font-mono text-brand-neon uppercase tracking-wider">Teil 1 (ca. 30 Min)</span>
                        <h3 class="text-xl font-bold font-syne text-white mt-1">Schnittstellen-Audit & Bottlenecks</h3>
                    </div>
                    <span class="bg-[#1F1F2E] text-brand-textMuted px-3 py-1 rounded-lg text-[10px] font-mono uppercase">Fokus: Datenfluss-Resilienz</span>
                </div>
                
                <div class="space-y-4">
                    <p class="text-xs text-brand-textMuted leading-relaxed">
                        Analysiere die oben visualisierte Daten-Pipeline. Welche <strong>zwei Schwachstellen</strong> blockieren die Skalierbarkeit unserer Systeme am meisten und führen zu massiven Synchronisations- und Datenkonsistenz-Problemen? Begründe deine Wahl aus architektonischer Sicht.
                    </p>
                    
                    <!-- Text Area Input -->
                    <div class="space-y-2">
                        <label for="task1_response" class="text-[11px] font-mono text-brand-textMuted uppercase tracking-wider block">Deine Analyse (Teil 1):</label>
                        <textarea id="task1_response" data-save="task1" placeholder="Fokussiere dich auf Daten-Silos, inkonsistente Formate und strukturelle Medienbrüche..." class="w-full min-h-[160px] bg-brand-darkBg border border-brand-border rounded-xl p-4 text-sm text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                    </div>
                </div>
            </div>

            <!-- ================= TASK 2 ================= -->
            <div class="bg-brand-darkCard border border-brand-border rounded-2xl p-6 md:p-8 space-y-8">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b border-brand-border pb-4 gap-4">
                    <div>
                        <span class="text-xs font-mono text-brand-neon uppercase tracking-wider">Teil 2 (ca. 30-45 Min)</span>
                        <h3 class="text-xl font-bold font-syne text-white mt-1">Lean Soll-Infrastruktur</h3>
                    </div>
                    <span class="bg-[#1F1F2E] text-brand-textMuted px-3 py-1 rounded-lg text-[10px] font-mono uppercase">Stack: Monday API, Notion API, Make/n8n, ChatGPT Vision</span>
                </div>

                <div class="space-y-4">
                    <p class="text-xs text-brand-textMuted leading-relaxed">
                        Entwirf eine automatisierte Soll-Infrastruktur. Verknüpfe die Systeme so, dass menschliche Fehler ausgeschlossen und manuelle Synchronisationen eliminiert werden.
                        <strong>Definiere 3 systemische Daten-Automationen:</strong>
                    </p>
                </div>

                <!-- Three Automation Panels -->
                <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
                    <!-- Automation 1 -->
                    <div class="bg-[#14141F] border border-brand-border/60 rounded-xl p-5 space-y-4">
                        <div class="text-xs font-bold text-brand-neon uppercase tracking-wider">⚡ Automation #1: Dubletten & Ingest-Validierung</div>
                        <div class="space-y-3">
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">System-Ziel:</label>
                                <input type="text" id="auto1_problem" data-save="auto1_p" placeholder="Z.B. Cross-Platform Duplikat-Verhinderung" class="w-full bg-brand-darkBg border border-brand-border rounded-lg px-3 py-2 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Ablauf (Trigger ➔ API-Validierung ➔ Actions):</label>
                                <textarea id="auto1_flow" data-save="auto1_f" placeholder="Welcher System-Event triggert? Wie wird die Eindeutigkeit (UUID/ID) geprüft?" class="w-full min-h-[100px] bg-brand-darkBg border border-brand-border rounded-lg p-3 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                            </div>
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">System-Verknüpfung (APIs):</label>
                                <input type="text" id="auto1_tools" data-save="auto1_t" placeholder="z.B. Monday webhook ➔ Make ➔ Engine DB check" class="w-full bg-brand-darkBg border border-brand-border rounded-lg px-3 py-2 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                        </div>
                    </div>

                    <!-- Automation 2 -->
                    <div class="bg-[#14141F] border border-brand-border/60 rounded-xl p-5 space-y-4">
                        <div class="text-xs font-bold text-brand-neon uppercase tracking-wider">⚡ Automation #2: Strukturierter Medien-Ingest</div>
                        <div class="space-y-3">
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">System-Ziel:</label>
                                <input type="text" id="auto2_problem" data-save="auto2_p" placeholder="Z.B. Unstrukturiertes Screenshot-Parsing via Vision KI" class="w-full bg-brand-darkBg border border-brand-border rounded-lg px-3 py-2 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Ablauf (Trigger ➔ API-Validierung ➔ Actions):</label>
                                <textarea id="auto2_flow" data-save="auto2_f" placeholder="Wie wandeln wir Bilddateien vollautomatisch in strukturierte JSON-Datensätze um?" class="w-full min-h-[100px] bg-brand-darkBg border border-brand-border rounded-lg p-3 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                            </div>
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">System-Verknüpfung (APIs):</label>
                                <input type="text" id="auto2_tools" data-save="auto2_t" placeholder="z.B. Discord/Form-Upload ➔ OpenAI Vision ➔ Notion Database Sync" class="w-full bg-brand-darkBg border border-brand-border rounded-lg px-3 py-2 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                        </div>
                    </div>

                    <!-- Automation 3 -->
                    <div class="bg-[#14141F] border border-brand-border/60 rounded-xl p-5 space-y-4">
                        <div class="text-xs font-bold text-brand-neon uppercase tracking-wider">⚡ Automation #3: Cross-Departmental Daten-Sync</div>
                        <div class="space-y-3">
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">System-Ziel:</label>
                                <input type="text" id="auto3_problem" data-save="auto3_p" placeholder="Z.B. Echtzeit-Abgleich Creative DB ↔ Ops Master" class="w-full bg-brand-darkBg border border-brand-border rounded-lg px-3 py-2 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Ablauf (Trigger ➔ API-Validierung ➔ Actions):</label>
                                <textarea id="auto3_flow" data-save="auto3_f" placeholder="Wie verhinderst du, dass Creative-Teams (Notion) und Planer (Monday) asynchron arbeiten?" class="w-full min-h-[100px] bg-brand-darkBg border border-brand-border rounded-lg p-3 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                            </div>
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">System-Verknüpfung (APIs):</label>
                                <input type="text" id="auto3_tools" data-save="auto3_t" placeholder="z.B. Notion-Database Webhooks ➔ Make ➔ Monday API V2" class="w-full bg-brand-darkBg border border-brand-border rounded-lg px-3 py-2 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Soll-Process Summary -->
                <div class="space-y-2">
                    <label for="task2_summary" class="text-[11px] font-mono text-brand-textMuted uppercase tracking-wider block">Soll-Infrastruktur Philosophie:</label>
                    <textarea id="task2_summary" data-save="task2_sum" placeholder="Was läuft vollständig automatisiert über Schnittstellen, wo bleibt menschliche Interaktion ganz bewusst gewollt (z.B. Quality Checks) – und wie sicherst du die System-Stabilität?" class="w-full min-h-[120px] bg-brand-darkBg border border-brand-border rounded-xl p-4 text-sm text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                </div>
            </div>

            <!-- ================= TASK 3 ================= -->
            <div class="bg-brand-darkCard border border-brand-border rounded-2xl p-6 md:p-8 space-y-6">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b border-brand-border pb-4 gap-4">
                    <div>
                        <span class="text-xs font-mono text-brand-neon uppercase tracking-wider">Teil 3 (ca. 20-30 Min)</span>
                        <h3 class="text-xl font-bold font-syne text-white mt-1">Infrastruktur-Priorisierung & MVP-Denken</h3>
                    </div>
                    <span class="bg-[#1F1F2E] text-brand-textMuted px-3 py-1 rounded-lg text-[10px] font-mono uppercase">Ressourcen-Constraint: Max. 2 Wochen Entwicklungszeit</span>
                </div>

                <div class="space-y-6">
                    <p class="text-xs text-brand-textMuted leading-relaxed">
                        Das Team hat 6 coole Ideen für künftige abteilungsübergreifende Prozess-Projekte gesammelt. Du hast aber <strong>nur zwei Wochen Entwicklungszeit</strong>. 
                        <strong>Wähle die 2 Projekte aus, die du als MVP (Minimum Viable Product) sofort baust, um den größten systemischen Hebel (Fehlerreduktion / Zeitgewinn) zu erzielen:</strong>
                    </p>

                    <!-- Interactive Choice Grid with updated Cross-Department projects -->
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-3">
                        <div class="project-card border border-brand-border bg-[#0E0E16]/40 p-4 rounded-xl flex flex-col justify-between hover:border-brand-border/80 transition-all">
                            <div>
                                <span class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block">PROJECT ID: 01</span>
                                <h4 class="text-sm font-bold text-white mt-1">Finance & Sourcing Matcher</h4>
                                <p class="text-[11px] text-brand-textMuted mt-1 leading-relaxed">Vollautomatische Schnittstelle, die Rechnungs-PDFs via KI einliest, mit Monday-Budgets abgleicht und für Finance bereitstellt.</p>
                            </div>
                        </div>
                        <div class="project-card border border-brand-border bg-[#0E0E16]/40 p-4 rounded-xl flex flex-col justify-between hover:border-brand-border/80 transition-all">
                            <div>
                                <span class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block">PROJECT ID: 02</span>
                                <h4 class="text-sm font-bold text-white mt-1">Multi-Client Looker Pipeline</h4>
                                <p class="text-[11px] text-brand-textMuted mt-1 leading-relaxed">Spiegelung aller Kampagnendaten aus Monday in standardisierte Looker-Studio Dashboards. Eliminiert händische Kundenberichte.</p>
                            </div>
                        </div>
                        <div class="project-card border border-brand-border bg-[#0E0E16]/40 p-4 rounded-xl flex flex-col justify-between hover:border-brand-border/80 transition-all">
                            <div>
                                <span class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block">PROJECT ID: 03</span>
                                <h4 class="text-sm font-bold text-white mt-1">Legal Contract Generator</h4>
                                <p class="text-[11px] text-brand-textMuted mt-1 leading-relaxed">Automatisierte Schnittstelle, die bei Monday-Statuswechsel rechtskonforme Verträge generiert, versendet und archiviert.</p>
                            </div>
                        </div>
                        <div class="project-card border border-brand-border bg-[#0E0E16]/40 p-4 rounded-xl flex flex-col justify-between hover:border-brand-border/80 transition-all">
                            <div>
                                <span class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block">PROJECT ID: 04</span>
                                <h4 class="text-sm font-bold text-white mt-1">Eskalations-Alert Engine</h4>
                                <p class="text-[11px] text-brand-textMuted mt-1 leading-relaxed">Automatischer Deadline-Checker in Monday, der bei Verzug Kaskaden-Warnungen via Slack an Team-Leads steuert.</p>
                            </div>
                        </div>
                        <div class="project-card border border-brand-border bg-[#0E0E16]/40 p-4 rounded-xl flex flex-col justify-between hover:border-brand-border/80 transition-all">
                            <div>
                                <span class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block">PROJECT ID: 05</span>
                                <h4 class="text-sm font-bold text-white mt-1">Automated Trend-Sourcing</h4>
                                <p class="text-[11px] text-brand-textMuted mt-1 leading-relaxed">API-Crawler, der Trending Creator filtert, bereinigt und direkt in die Notion-Wissensdatenbank für Creatives einspeist.</p>
                            </div>
                        </div>
                        <div class="project-card border border-brand-border bg-[#0E0E16]/40 p-4 rounded-xl flex flex-col justify-between hover:border-brand-border/80 transition-all">
                            <div>
                                <span class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block">PROJECT ID: 06</span>
                                <h4 class="text-sm font-bold text-white mt-1">Central Input Lead Gate</h4>
                                <p class="text-[11px] text-brand-textMuted mt-1 leading-relaxed">Einheitlicher Daten-Ingest für alle Partner-Anfragen zur radikalen Vermeidung von Datensilos und Duplikaten.</p>
                            </div>
                        </div>
                    </div>

                    <!-- Input fields for selected options -->
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Gewählte 2 System-MVPs & Begründung:</label>
                            <textarea id="task3_mvp" data-save="task3_mvp_text" placeholder="Welche zwei wählst du aus? Was ist das unschlagbare Argument (Skalierbarkeit, System-ROI)?" class="w-full min-h-[120px] bg-brand-darkBg border border-brand-border rounded-xl p-4 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                        </div>
                        <div>
                            <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Welche lässt du bewusst liegen?</label>
                            <textarea id="task3_abandon" data-save="task3_abandon_text" placeholder="Welche stellst du knallhart zurück und warum sind sie aktuell Zeitverschwendung?" class="w-full min-h-[120px] bg-brand-darkBg border border-brand-border rounded-xl p-4 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ================= TASK 4 ================= -->
            <div class="bg-brand-darkCard border border-brand-border rounded-2xl p-6 md:p-8 space-y-6">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b border-brand-border pb-4 gap-4">
                    <div>
                        <span class="text-xs font-mono text-red-400 uppercase tracking-wider">Teil 4 (ca. 20 Min)</span>
                        <h3 class="text-xl font-bold font-syne text-white mt-1">Schnittstellen- & Wissens-Chaos</h3>
                    </div>
                    <span class="bg-red-500/10 text-red-400 px-3 py-1 rounded-lg text-[10px] font-mono uppercase border border-red-500/20 animate-pulse">Abteilungsübergreifende Challenge</span>
                </div>

                <div class="space-y-4">
                    <blockquote class="italic text-brand-textMuted border-l-2 border-brand-neon pl-4 text-sm leading-relaxed">
                        „Montagmorgen. Das Creative-Team fordert neue Video-Ideen für Skripte, die eigentlich über eine API-Crawler-Automation in eine Notion-Wissensdatenbank laufen sollten – doch die Schnittstelle bricht wegen eines API-Rate-Limits komplett ab. Gleichzeitig wartet die Finance-Abteilung auf den automatisierten Monats-Report, weil Daten zwischen Monday und unserem Abrechnungs-Tool fehlerhafte Formate aufweisen und der Abgleich hakt.“
                    </blockquote>
                    <p class="text-xs text-brand-textMuted">
                        Als Brückenbauer zwischen den Abteilungen ist das dein Moment. Zeige uns, wie du strukturiert Fehler suchst und Abläufe am Leben hältst.
                    </p>

                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">1. Ad-hoc Behebung (Datenfluss retten):</label>
                            <textarea id="task4_rescue" data-save="task4_rescue_text" placeholder="Wie fängst du den Fehler pragmatisch für die Creatives ab? Wie hilfst du Finance ad-hoc, um an die Abrechnungsdaten zu kommen?" class="w-full min-h-[140px] bg-brand-darkBg border border-brand-border rounded-xl p-4 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                        </div>
                        <div>
                            <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">2. Nachhaltiges Design (Skalierung & API):</label>
                            <textarea id="task4_prevent" data-save="task4_prevent_text" placeholder="Wie strukturierst du die Notion-Datenbank, den Content-Crawler und die Finanz-Schnittstelle langfristig, um Formatfehler und API-Sperren auszuschließen?" class="w-full min-h-[140px] bg-brand-darkBg border border-brand-border rounded-xl p-4 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ================= TASK 5 ================= -->
            <div class="bg-brand-darkCard border border-brand-border rounded-2xl p-6 md:p-8 space-y-6">
                <div class="flex flex-col md:flex-row justify-between items-start md:items-center border-b border-brand-border pb-4 gap-4">
                    <div>
                        <span class="text-xs font-mono text-brand-neon uppercase tracking-wider">Teil 5 (ca. 20 Min)</span>
                        <h3 class="text-xl font-bold font-syne text-white mt-1">Der systemische Skalierungs-Hebel</h3>
                    </div>
                    <span class="bg-[#1F1F2E] text-brand-textMuted px-3 py-1 rounded-lg text-[10px] font-mono uppercase">Eigene Idee / Freestyle</span>
                </div>

                <div class="space-y-4">
                    <p class="text-xs text-brand-textMuted leading-relaxed">
                        Wenn du dir den gesamten Agenturalltag bei einer Social-First-Agentur vorstellst: Wo siehst du das größte Potenzial für eine **neue abteilungsübergreifende Schnittstelle**, die massive Reibung zwischen Teams (z.B. Account Management, Creative Production, Legal, Finance) vollständig auflöst?
                    </p>

                    <div class="space-y-4">
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Welches abteilungsübergreifende Problem wird gelöst?</label>
                                <input type="text" id="task5_problem" data-save="task5_p_text" placeholder="Z. B. Reibungsverlust zwischen Creative-Freigaben und Account-Managern" class="w-full bg-brand-darkBg border border-brand-border rounded-xl px-4 py-3 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                            <div>
                                <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Was ist der messbare System-Nutzen (ROI)?</label>
                                <input type="text" id="task5_benefit" data-save="task5_b_text" placeholder="Z. B. Keine manuellen Updates mehr, Einsparung von 5 Stunden Absprachen/Woche" class="w-full bg-brand-darkBg border border-brand-border rounded-xl px-4 py-3 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()">
                            </div>
                        </div>
                        <div>
                            <label class="text-[10px] font-mono text-brand-textMuted uppercase tracking-wider block mb-1">Der systemische Ablauf Schritt-für-Schritt:</label>
                            <textarea id="task5_flow" data-save="task5_f_text" placeholder="Beschreibe kurz den genauen Datenfluss, die beteiligten APIs/Tools und die systemischen Übergabepunkte." class="w-full min-h-[120px] bg-brand-darkBg border border-brand-border rounded-xl p-4 text-xs text-white neon-border-focus transition-all duration-200" oninput="updateProgress()"></textarea>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SUBMIT & EXPORT PORTAL -->
        <section class="bg-gradient-to-br from-[#0F0F1A] to-[#0A0A0F] border-2 border-brand-neon/20 rounded-3xl p-8 relative overflow-hidden text-center space-y-6">
            <div class="absolute -top-16 -right-16 w-36 h-36 bg-brand-neon/10 rounded-full blur-2xl"></div>
            
            <div class="max-w-xl mx-auto space-y-3">
                <span class="text-xs text-brand-neon font-mono uppercase tracking-widest block font-bold">// JETZT EXPORTIEREN</span>
                <h3 class="text-2xl md:text-3xl font-extrabold font-syne text-white">Abgabe generieren</h3>
                <p class="text-xs text-brand-textMuted leading-relaxed">
                    Deine Antworten wurden kontinuierlich lokal im Browser gesichert. Drücke auf den Button unten, um deine Abgabe als sauber formatiertes **Markdown-Dokument (.md)** herunterzuladen oder direkt zu kopieren. Schicke dieses Dokument einfach an deinen Kontakt bei DEPARTD.
                </p>
            </div>

            <div class="flex flex-col sm:flex-row gap-4 justify-center items-center pt-4">
                <button onclick="exportMarkdownFile()" class="w-full sm:w-auto bg-brand-neon hover:bg-white text-black font-extrabold px-8 py-4 rounded-xl text-sm transition-all duration-300 transform hover:-translate-y-1 hover:shadow-[0_0_25px_rgba(228,255,0,0.35)] flex items-center justify-center space-x-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2.5"><path stroke-linecap="round" stroke-linejoin="round" d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4" /></svg>
                    <span>Abgabe herunterladen (.md)</span>
                </button>
                <button onclick="copySubmissionToClipboard()" class="w-full sm:w-auto bg-[#1F1F2E] hover:bg-brand-neon hover:text-black border border-brand-border text-xs font-bold py-4 px-6 rounded-xl transition-all duration-300 flex items-center justify-center space-x-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M8 5H6a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2v-1M8 5a2 2 0 002 2h2a2 2 0 002-2M8 5a2 2 0 012-2h2a2 2 0 012 2m0 0h2a2 2 0 012 2v3m2 4H10m0 0l3-3m-3 3l3 3" /></svg>
                    <span>In Zwischenablage kopieren</span>
                </button>
            </div>
            
            <div class="text-[10px] text-brand-textMuted font-mono">
                Sicherer, lokaler Export &bull; Keine Serverübertragung deiner Daten
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="px-6 py-4 md:px-12 border-t border-brand-border/40 backdrop-blur-md bg-brand-darkBg/80 flex flex-col md:flex-row items-center justify-between z-50 gap-4">
        <div class="text-xs font-mono text-brand-textMuted">
            DEPARTD &copy; 2026 &bull; Processes & Automation Testcase
        </div>
        <div class="flex items-center space-x-4 text-xs text-brand-textMuted">
            <a href="#" onclick="resetAllFields(event)" class="hover:text-red-400 transition-colors font-mono">Formular zurücksetzen</a>
        </div>
    </footer>

    <!-- Notification Toast -->
    <div id="toast" class="fixed top-6 right-6 z-[100] transform translate-y-[-100px] opacity-0 transition-all duration-300 bg-brand-darkCard border border-brand-neon text-white px-5 py-3.5 rounded-xl shadow-2xl flex items-center space-x-3 pointer-events-none">
        <span class="text-brand-neon text-base">✓</span>
        <span class="text-xs font-bold" id="toast-text">Erfolgreich kopiert!</span>
    </div>

    <script>
        // Custom flow steps details for the Systemic Pipeline Simulator
        const flowSteps = {
            1: {
                title: "Datenquellen & Fragmentierung",
                desc: "Daten strömen völlig unstrukturiert über Webformulare, Mail-Postfächer, DMs und manuelle Recherchen ein. Es existiert kein zentrales Gateway oder einheitlicher Ingest-Parser.",
                problem: "Strikte Daten-Silos. Operative Teams fischen Daten händisch aus Drittsystemen, anstatt dass diese strukturiert, validiert und konsolidiert im Master-System Monday.com eintreffen.",
                risk: "🔴 Extrem hoch",
                clicks: "Manuell & Dezentral"
            },
            2: {
                title: "Daten-Inkonsistenz & Dubletten",
                desc: "Recherchierte und eingehende Profile werden ohne automatische ID-Validierung direkt in Monday Boards eingepflegt. Es gibt keinen automatischen Dubletten-Check im Hintergrund.",
                problem: "Identische Creator oder Leads werden mehrfach erfasst. Dies führt zu chaotischer Datenpflege, asynchronen Absprachen und im schlimmsten Fall zu unprofessioneller Mehrfach-Kontaktaufnahme.",
                risk: "🔴 Extrem hoch",
                clicks: "Keine Validierung"
            },
            3: {
                title: "Unstrukturierter Medienbruch",
                desc: "Die wertvollen Reichweiten- und Leistungsdaten werden unstrukturiert als Bilddatei (Screenshot) per Mail oder WhatsApp eingereicht.",
                problem: "Wertvolle System-Daten liegen als totes Bildformat vor. Es verstreicht Zeit mit dem manuellen Abtippen und Überführen der KPIs in Zahlenspalten, was fehleranfällig ist.",
                risk: "🟡 Hoch",
                clicks: "Händisches Abtippen"
            },
            4: {
                title: "Isolierte Kategorisierung (Silos)",
                desc: "Jedes Profil wird manuell nach Gefühl oder Erfahrung einer Kategorie wie Beauty, Gaming oder Food zugeordnet.",
                problem: "Keine standardisierten, regelbasierten Klassifizierungen. Suchen von Creatives scheitern oft, da die Notion-Wissensdatenbank und Monday unterschiedliche Tags nutzen. Daten-Inkonsistenz.",
                risk: "🟡 Medium",
                clicks: "Mangelnde Standardisierung"
            }
        };

        // Switch Simulator details
        function selectFlowStep(stepId) {
            document.querySelectorAll('.flow-btn').forEach(btn => {
                btn.classList.remove('border-brand-neon/40', 'bg-brand-neon/5', 'active');
                btn.classList.add('border-brand-border', 'bg-[#0E0E16]/30');
                btn.querySelector('.step-badge').classList.replace('text-brand-neon', 'text-brand-textMuted');
            });
            
            const activeBtn = document.getElementById(`btn-flow-${stepId}`);
            activeBtn.classList.add('border-brand-neon/40', 'bg-brand-neon/5', 'active');
            activeBtn.classList.remove('border-brand-border', 'bg-[#0E0E16]/30');
            activeBtn.querySelector('.step-badge').classList.replace('text-brand-textMuted', 'text-brand-neon');

            const info = flowSteps[stepId];
            document.getElementById('flow-title').innerText = info.title;
            document.getElementById('flow-desc').innerText = info.desc;
            document.getElementById('flow-problem').innerText = info.problem;
            document.getElementById('flow-risk').innerText = info.risk;
            document.getElementById('flow-clicks').innerText = info.clicks;
        }

        // Setup background autosave to protect candidate inputs silently
        const inputElements = document.querySelectorAll('[data-save]');

        // Load cached inputs silently on launch
        window.addEventListener('load', () => {
            inputElements.forEach(el => {
                const cachedVal = localStorage.getItem('departd_case_struct_' + el.getAttribute('data-save'));
                if (cachedVal) {
                    el.value = cachedVal;
                }
            });
        });

        // Event listeners to save on change/input silently in the background
        inputElements.forEach(el => {
            el.addEventListener('input', () => {
                localStorage.setItem('departd_case_struct_' + el.getAttribute('data-save'), el.value);
            });
        });

        // Silent progress tracker bypass (keeps UI clean and focused)
        function updateProgress() {}

        // Helper to trigger toast messages without browser alerts
        function triggerToast(message) {
            const toast = document.getElementById('toast');
            document.getElementById('toast-text').innerText = message;
            toast.classList.remove('translate-y-[-100px]', 'opacity-0');
            toast.classList.add('translate-y-0', 'opacity-100');
            
            setTimeout(() => {
                toast.classList.add('translate-y-[-100px]', 'opacity-0');
                toast.classList.remove('translate-y-0', 'opacity-100');
            }, 2500);
        }

        // Reset Workspace data helper
        function resetAllFields(e) {
            e.preventDefault();
            if (confirm("Möchtest du wirklich alle eingetragenen Antworten löschen und neu anfangen?")) {
                inputElements.forEach(el => {
                    el.value = "";
                    localStorage.removeItem('departd_case_struct_' + el.getAttribute('data-save'));
                });
                triggerToast("Workspace erfolgreich zurückgesetzt!");
            }
        }

        // Generate Structured Markdown Report
        function generateMarkdownString() {
            const t1 = document.getElementById('task1_response').value || "Noch keine Antwort hinterlegt.";
            
            const a1_p = document.getElementById('auto1_problem').value || "---";
            const a1_f = document.getElementById('auto1_flow').value || "---";
            const a1_t = document.getElementById('auto1_tools').value || "---";
            
            const a2_p = document.getElementById('auto2_problem').value || "---";
            const a2_f = document.getElementById('auto2_flow').value || "---";
            const a2_t = document.getElementById('auto2_tools').value || "---";
            
            const a3_p = document.getElementById('auto3_problem').value || "---";
            const a3_f = document.getElementById('auto3_flow').value || "---";
            const a3_t = document.getElementById('auto3_tools').value || "---";

            const t2_sum = document.getElementById('task2_summary').value || "Noch keine Antwort hinterlegt.";
            
            const t3_mvp = document.getElementById('task3_mvp').value || "Noch keine Antwort hinterlegt.";
            const t3_abandon = document.getElementById('task3_abandon').value || "Noch keine Antwort hinterlegt.";
            
            const t4_rescue = document.getElementById('task4_rescue').value || "Noch keine Antwort hinterlegt.";
            const t4_prevent = document.getElementById('task4_prevent').value || "Noch keine Antwort hinterlegt.";
            
            const t5_prob = document.getElementById('task5_problem').value || "---";
            const t5_ben = document.getElementById('task5_benefit').value || "---";
            const t5_flow = document.getElementById('task5_flow').value || "Noch keine Antwort hinterlegt.";

            return `# 🧩 DEPARTD · Testaufgabe Abgabe
## Werkstudent:in – Processes & Automation Architect

---

## 📝 Teil 1: Schnittstellen-Audit & Bottlenecks

### Deine Analyse der Schwachstellen & Engpässe:
${t1}

---

## ⚡ Teil 2: Lean Soll-Infrastruktur

### Automation #1: Dubletten & Ingest-Validierung
* **System-Ziel:** ${a1_p}
* **Schnittstellen (APIs):** ${a1_t}
* **Schnittstellen-Ablauf:**
${a1_f}

### Automation #2: Strukturierter Medien-Ingest
* **System-Ziel:** ${a2_p}
* **Schnittstellen (APIs):** ${a2_t}
* **Schnittstellen-Ablauf:**
${a2_f}

### Automation #3: Cross-Departmental Daten-Sync
* **System-Ziel:** ${a3_p}
* **Schnittstellen (APIs):** ${a3_t}
* **Schnittstellen-Ablauf:**
${a3_f}

### Soll-Infrastruktur Philosophie:
* **Was läuft vollautomatisiert, was bleibt manuell und warum?**
${t2_sum}

---

## 📊 Teil 3: Infrastruktur-Priorisierung & MVP-Denken (2-Wochen-Constraint)

### Ausgewählte MVPs & Begründung:
${t3_mvp}

### Bewusst zurückgestellte Projekte & Rationale:
${t3_abandon}

---

## 🚨 Teil 4: Schnittstellen- & Wissens-Chaos (Notfall-Simulation)

### 1. Ad-hoc Behebung (Datenfluss sichern):
${t4_rescue}

### 2. Nachhaltiger Workflow (Prävention & Scale):
${t4_prevent}

---

## 💡 Teil 5: Der systemische Skalierungs-Hebel (Dein eigener Workflow)

* **Gelöstes Problem:** ${t5_prob}
* **Erwarteter System-Nutzen / ROI:** ${t5_ben}

### Ablauf des Workflows:
${t5_flow}

---
*Generiert mit dem DEPARTD Live Workspace &bull; ${new Date().toLocaleDateString('de-DE')}*`;
        }

        // Export Markdown file trigger
        function exportMarkdownFile() {
            const mdContent = generateMarkdownString();
            const blob = new Blob([mdContent], { type: 'text/markdown;charset=utf-8;' });
            const link = document.createElement("a");
            
            if (link.download !== undefined) {
                const url = URL.createObjectURL(blob);
                link.setAttribute("href", url);
                link.setAttribute("download", "departd_testaufgabe_processes_abgabe.md");
                link.style.visibility = 'hidden';
                document.body.appendChild(link);
                link.click();
                document.body.removeChild(link);
                triggerToast("Abgabe erfolgreich heruntergeladen!");
            }
        }

        // Copy markdown string to clipboard (using robust fallback)
        function copySubmissionToClipboard() {
            const mdContent = generateMarkdownString();
            const el = document.createElement('textarea');
            el.value = mdContent;
            document.body.appendChild(el);
            el.select();
            document.execCommand('copy');
            document.body.removeChild(el);
            triggerToast("Abgabe in Zwischenablage kopiert!");
        }
    </script>
</body>
</html>
