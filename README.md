<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ShokzHear Singapore BD Guideline</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Chosen Palette: Warm Neutrals with Blue Accent (Tailwind grays, blues, and yellows) -->
    <!-- Application Structure Plan: The single-page application (SPA) uses a tab-based structure. Users can switch between "Home", "Negotiation Process", "Key Details", and "Market Exception". This structure is chosen because the source information is primarily a process and rule guide, prioritizing organized flow over data visualization. The tabs offer a clear, systematic user path, allowing potential distributors to selectively find information, which is more intuitive than a long scrolling page. JavaScript handles navigation clicks to dynamically show/hide the content panels. -->
    <!-- Visualization & Content Choices: The source report contains no quantitative data, so Chart.js or Plotly are not used. Information is presented using structured HTML and Tailwind CSS. 1. Negotiation Process -> Goal: Organize/Inform -> Presentation: Visual steps using Tailwind CSS cards and Unicode numbering (1️⃣, 2️⃣, 3️⃣) -> Interaction: None (controlled by main tab navigation) -> Justification: Clearly presents linear steps. 2. Key Details -> Goal: Inform -> Presentation: Info cards with Unicode icons (✉️, 📍) -> Interaction: Added "Copy" button next to the email address (JavaScript) -> Justification: Highlights core rules and provides utility. 3. Market Exception -> Goal: Inform/Warn -> Presentation: Highlighted card using alert colors (yellow/red) and ⚠️ icon -> Interaction: None -> Justification: Clearly communicates critical restrictions. A new card highlights Engineer Support (Audition/Fitting). -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, 'Noto Sans', sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <div class="container mx-auto max-w-4xl p-4 sm:p-6 lg:p-8">
        
        <header class="mb-6">
            <h1 class="text-3xl font-bold text-gray-900 mb-2">ShokzHear Singapore Landing Page</h1>
        </header>

        <nav class="mb-6 bg-white rounded-lg shadow-sm">
            <div role="tablist" class="flex flex-wrap border-b border-gray-200">
                <button role="tab" data-tab="content-home" class="nav-tab px-4 py-3 sm:px-6 font-medium text-sm sm:text-base text-gray-600 border-b-2 border-transparent hover:text-blue-600 hover:border-blue-600 whitespace-nowrap">
                    Home
                </button>
                <button role="tab" data-tab="content-process" class="nav-tab px-4 py-3 sm:px-6 font-medium text-sm sm:text-base text-gray-600 border-b-2 border-transparent hover:text-blue-600 hover:border-blue-600 whitespace-nowrap">
                    Get in touch
                </button>
                <button role="tab" data-tab="content-details" class="nav-tab px-4 py-3 sm:px-6 font-medium text-sm sm:text-base text-gray-600 border-b-2 border-transparent hover:text-blue-600 hover:border-blue-600 whitespace-nowrap">
                    Key Details
                </button>
                <button role="tab" data-tab="content-exception" class="nav-tab px-4 py-3 sm:px-6 font-medium text-sm sm:text-base text-gray-600 border-b-2 border-transparent hover:text-blue-600 hover:border-blue-600 whitespace-nowrap">
                    Market Exception
                </button>
            </div>
        </nav>

        <main id="tab-content" class="bg-white p-5 sm:p-8 rounded-lg shadow">

            <section id="content-home" role="tabpanel" class="tab-panel space-y-4">
                <h2 class="text-2xl font-semibold text-gray-900 mb-4">Welcome to ShokzHear Singapore landing page</h2>
                <p class="text-gray-700 leading-relaxed">
                    Thank you for your interest in ShokzHear Singapore market. This guide provides a overview of the actions needed if you are interested in our product or looking for collaboration opportunities.
                </p>
                <p class="text-gray-700 leading-relaxed">
                    The primary contact is Mr. Liu Fayang, our algorithm engineer based in Singapore. All initial contact would be handled by him. Notice that our physical reception and goods collection point are located in Shenzhen, China.
                </p>
                <p class="text-gray-700 leading-relaxed">
                    Please use the navigation tabs above to explore different sections, including the how to get in touch and current business status.
                </p>
                <div class="mt-6 p-4 bg-blue-50 border-l-4 border-blue-500 rounded-r-lg">
                    <p class="font-medium text-blue-800">
                        We are looking for interested distributors, and you are welcome to contact us even if you do not have an existing partnership with us.
                    </p>
                </div>
            </section>

            <section id="content-process" role="tabpanel" class="tab-panel hidden space-y-4">
                <h2 class="text-2xl font-semibold text-gray-900 mb-4">How to get in touch</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    This section guides you through the complete process from first contact to final goods collection. We break it down into three main steps for clarity on how to start a partnership with us.
                </p>
                
                <div class="space-y-6">
                    <div class="flex items-start space-x-4">
                        <div class="flex-shrink-0 flex items-center justify-center h-10 w-10 rounded-full bg-blue-600 text-white font-bold text-xl">
                            1
                        </div>
                        <div>
                            <h3 class="text-lg font-semibold text-gray-900">Initial Contact</h3>
                            <p class="text-gray-700 mt-1">
                                If you are interested in collaboration opportunities, please contact Mr. Liu Fayang via email for preliminary discussions.
                            </p>
                            <p class="text-gray-700 mt-2 font-medium">
                                Contact: Liu Fayang (Personal Capacity)
                            </p>
                            <p class="text-gray-700 mt-1">
                                Email: <code class="text-blue-700">liufayang@shokz.com</code>
                            </p>
                        </div>
                    </div>

                    <div class="flex items-start space-x-4">
                        <div class="flex-shrink-0 flex items-center justify-center h-10 w-10 rounded-full bg-blue-600 text-white font-bold text-xl">
                            2
                        </div>
                        <div>
                            <h3 class="text-lg font-semibold text-gray-900">In-Depth Discussion (Store Visit)</h3>
                            <p class="text-gray-700 mt-1">
                                If you have time and wish to learn more about the product and collaboration details, we invite you to visit our fitting center in Shenzhen.
                            </p>
                            <p class="text-gray-700 mt-2 font-medium">
                                Location: Shokz Hearing Aid Fitting Center
                            </p>
                            <p class="text-gray-700 mt-1">
                                Address: No. 4221 Xili Lake Road, Nanshan District, Shenzhen, Guangdong Province
                            </p>
                            <p class="text-gray-600 italic mt-1">
                                * Staff will be available at the store to receive you.
                            </p>
                        </div>
                    </div>

                    <div class="flex items-start space-x-4">
                        <div class="flex-shrink-0 flex items-center justify-center h-10 w-10 rounded-full bg-blue-600 text-white font-bold text-xl">
                            3
                        </div>
                        <div>
                            <h3 class="text-lg font-semibold text-gray-900">Cooperation & Goods Collection</h3>
                            <p class="text-gray-700 mt-1">
                                Upon official collaboration, all goods must be collected by the distributor in Shenzhen.
                            </p>
                            <p class="text-gray-700 mt-2 font-medium">
                                Collection Point: Shenzhen
                            </p>
                            <p class="text-gray-700 mt-1">
                                Method: Distributor self-collection
                            </p>
                        </div>
                    </div>
                </div>
            </section>

            <section id="content-details" role="tabpanel" class="tab-panel hidden space-y-4">
                <h2 class="text-2xl font-semibold text-gray-900 mb-4">Key Information At a Glance</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    Before starting the process, please review the critical information points below, covering contact details, partnership requirements, and logistics.
                </p>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-5">
                    <div class="bg-gray-50 rounded-lg p-5 border border-gray-200">
                        <h3 class="text-lg font-semibold text-gray-900 mb-2">✉️ Primary Contact</h3>
                        <p class="text-gray-700">
                            Mr. Liu Fayang<br>
                            <span id="email-address" class="text-blue-700 font-medium">liufayang@shokz.com</span>
                        </p>
                        <button id="copy-email-btn" class="mt-3 inline-flex items-center px-3 py-1.5 border border-gray-300 shadow-sm text-sm font-medium rounded-md text-gray-700 bg-white hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-blue-500">
                            Copy Email
                        </button>
                    </div>

                    <div class="bg-blue-50 rounded-lg p-5 border border-blue-400">
                        <h3 class="text-lg font-semibold text-blue-800 mb-2">🧑‍🔧 Engineer Support Services (Singapore)</h3>
                        <p class="text-blue-700">
                           Our engineer (based in Singapore) can provide the following technical support:
                        </p>
                        <ul class="list-disc list-inside text-blue-700 mt-2 ml-4 space-y-1 text-sm">
                            <li>Sample Audition/Trial</li>
                            <li>Hearing Aid Fitting/Matching Support</li>
                        </ul>
                    </div>

                    <div class="bg-gray-50 rounded-lg p-5 border border-gray-200">
                        <h3 class="text-lg font-semibold text-gray-900 mb-2">🤝 Partnership Status</h3>
                        <p class="text-gray-700">
                            We welcome new distributors. The current negotiation is conducted on a personal level, and you <strong class="font-semibold">do not</strong> need to have a prior official partnership with us.
                        </p>
                    </div>

                    <div class="bg-gray-50 rounded-lg p-5 border border-gray-200">
                        <h3 class="text-lg font-semibold text-gray-900 mb-2">🚚 Logistics & Collection</h3>
                        <p class="text-gray-700">
                            All goods must be <strong class="font-semibold text-blue-700">self-collected by the distributor</strong> in <strong class="font-semibold">Shenzhen</strong>.
                        </p>
                    </div>
                </div>
            </section>

            <section id="content-exception" role="tabpanel" class="tab-panel hidden space-y-4">
                <h2 class="text-2xl font-semibold text-gray-900 mb-4">Market Exception: Singapore</h2>
                <p class="text-gray-700 leading-relaxed mb-6">
                    This is a critical section for distributors interested in the Singapore market. Please read the following strict restrictions on market access carefully.
                </p>

                <div class="bg-yellow-50 border-l-4 border-yellow-400 p-5 rounded-r-lg">
                    <div class="flex">
                        <div class="flex-shrink-0">
                            <span class="text-2xl" aria-hidden="true">⚠️</span>
                        </div>
                        <div class="ml-3">
                            <h3 class="text-lg font-semibold text-yellow-800">Strict Restriction: Does not allow public sale</h3>
                            <div class="mt-2 text-sm text-yellow-700 space-y-2">
                                <p>
                                    Core Reason: Singapore currently <strong class="font-semibold">does not have a medical device sales license</strong>.
                                </p>
                                <p>
                                    Therefore, hearing aid products <strong class="font-semibold text-red-700">cannot be listed or sold publicly</strong> in Singapore.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="mt-6 bg-blue-50 border-l-4 border-blue-400 p-5 rounded-r-lg">
                    <div class="flex">
                        <div class="flex-shrink-0">
                            <span class="text-2xl" aria-hidden="true">💡</span>
                        </div>
                        <div class="ml-3">
                            <h3 class="text-lg font-semibold text-blue-800">Exception: Small-Scale Market Exploration</h3>
                            <div class="mt-2 text-sm text-blue-700 space-y-2">
                                <p>
                                    <strong class="font-semibold">However</strong>, if you are an existing partner or a distributor looking to <strong class="font-semibold">explore the market on a small scale</strong>, we can discuss this <strong class="font-semibold text-blue-900">case by case</strong>.
                                </p>
                                <p>
                                    This does not grant permission for public sales, but for discussing the feasibility of market exploration within a compliant framework, utilizing the local support for audition and fitting provided by our engineer.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

        </main>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const tabs = document.querySelectorAll('button[role="tab"]');
            const panels = document.querySelectorAll('section[role="tabpanel"]');
            const copyBtn = document.getElementById('copy-email-btn');
            const emailAddress = document.getElementById('email-address').innerText;

            const activeTabClasses = ['bg-blue-600', 'text-white'];
            const inactiveTabClasses = ['text-gray-600', 'hover:text-blue-600', 'hover:border-blue-600'];

            function showTab(tabId) {
                panels.forEach(panel => {
                    if (panel.id === tabId) {
                        panel.classList.remove('hidden');
                    } else {
                        panel.classList.add('hidden');
                    }
                });

                tabs.forEach(tab => {
                    if (tab.dataset.tab === tabId) {
                        tab.classList.add(...activeTabClasses);
                        tab.classList.remove(...inactiveTabClasses);
                        tab.setAttribute('aria-selected', 'true');
                    } else {
                        tab.classList.remove(...activeTabClasses);
                        tab.classList.add(...inactiveTabClasses);
                        tab.setAttribute('aria-selected', 'false');
                    }
                });
            }

            tabs.forEach(tab => {
                tab.addEventListener('click', (e) => {
                    e.preventDefault();
                    showTab(e.currentTarget.dataset.tab);
                });
            });

            if (copyBtn) {
                copyBtn.addEventListener('click', () => {
                    try {
                        const tempTextarea = document.createElement('textarea');
                        tempTextarea.value = emailAddress;
                        tempTextarea.style.position = 'absolute';
                        tempTextarea.style.left = '-9999px';
                        document.body.appendChild(tempTextarea);
                        tempTextarea.select();
                        document.execCommand('copy');
                        document.body.removeChild(tempTextarea);

                        const originalText = copyBtn.innerText;
                        copyBtn.innerText = 'Copied!';
                        copyBtn.disabled = true;
                        setTimeout(() => {
                            copyBtn.innerText = originalText;
                            copyBtn.disabled = false;
                        }, 2000);
                    } catch (err) {
                        console.error('Failed to copy email: ', err);
                    }
                });
            }
            
            showTab('content-home');
        });
    </script>
</body>
</html>
