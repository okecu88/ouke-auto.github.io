<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>郑州欧克汽车零部件有限公司-汽车零部件制造商</title>
    <!-- 稳定的 Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#E63946',
                        secondary: '#457B9D',
                        dark: '#1D3557',
                        light: '#F1FAEE',
                    },
                    fontFamily: {
                        sans: ['Inter','system-ui','sans-serif'],
                    },
                }
            }
        }
    </script>
    
    <style type="text/tailwindcss">
        /* 自定义样式 - 兼容所有环境 */
        .content-auto { content-visibility: auto; }
        .text-shadow { text-shadow: 0 2px 4px rgba(0,0,0,0.1); }
        .transition-custom { transition: all 0.3s ease-in-out; }
        .product-card {
            @apply bg-white rounded-lg shadow-md hover:shadow-xl transition-custom p-4 border border-gray-100;
        }
        .product-card-placeholder {
            @apply bg-gray-50 rounded-lg shadow-md hover:shadow-xl transition-custom p-4 border border-gray-100 flex items-center justify-center h-full min-h-[200px] text-gray-400;
        }
        .brand-tag {
            @apply bg-white rounded-lg shadow-sm p-3 text-center hover:shadow-md hover:bg-primary/5 transition-custom border border-gray-100;
        }
        .ecu-tag {
            @apply bg-white rounded-md p-2 text-center border border-gray-200 text-sm;
        }
        .supplement-text {
            @apply text-center text-gray-600 py-3 italic;
        }
        html { scroll-behavior: smooth; }
        .image-modal {
            @apply fixed inset-0 bg-black/95 z-50 flex items-center justify-center hidden;
        }
        .modal-content {
            @apply max-w-5xl max-h-[95vh] p-2;
        }
        .modal-image {
            @apply w-full h-auto max-h-[90vh] object-contain;
        }
        .close-btn {
            @apply absolute top-4 right-4 text-white text-primary transition-custom z-10;
        }
        .qrcode-box {
            @apply bg-white p-4 rounded-lg shadow-md text-center;
        }
        .factory-card {
            @apply bg-white rounded-lg shadow-md overflow-hidden;
        }
        .factory-img {
            @apply h-60 w-full object-cover;
        }
    </style>
</head>
<body class="font-sans text-dark bg-white">

<!-- 导航栏 - 含工厂实景入口（已添加公司LOGO） -->
<nav id="navbar" class="fixed w-full z-50 transition-custom py-4 bg-dark/90">
    <div class="container mx-auto px-4 md:px-8 flex justify-between items-center">
        <a href="#" class="text-2xl font-bold text-shadow text-white flex items-center">
            <!-- 公司LOGO -->
            <img src="https://p9-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/73271115224dbebc11557709f71446.png~tplv-a9rns2rl98-image.png?lk3s=8e244e95&rcl=20260320162540CE54F6183B0F9F0B5D53&rrcfp=dafada99&x-expires=2090219140&x-signature=SVekwt1q9CEMS9R7vJgPcAIWLdo%3D" 
                 alt="欧克汽车零部件LOGO" 
                 class="h-8 w-auto mr-2 object-contain">
            欧克汽车零部件
        </a>
        <div class="hidden md:flex space-x-8">
            <a href="#home" class="text-white hover:text-secondary transition-custom">首页</a>
            <a href="#about" class="text-white hover:text-secondary transition-custom">关于我们</a>
            <a href="#services" class="text-white hover:text-secondary transition-custom">核心业务</a>
            <a href="#factory" class="text-white hover:text-secondary transition-custom">工厂实景</a>
            <a href="#equipment" class="text-white hover:text-secondary transition-custom">生产设备</a>
            <a href="#series" class="text-white hover:text-secondary transition-custom">适配车型</a>
            <a href="#products" class="text-white hover:text-secondary transition-custom">产品展示</a>
            <a href="#contact" class="text-white hover:text-secondary transition-custom">联系我们</a>
        </div>
        <button id="menuBtn" class="md:hidden text-white text-2xl">
            <i class="fa-solid fa-bars"></i>
        </button>
    </div>
    <div id="mobileMenu" class="md:hidden hidden bg-white shadow-lg absolute w-full">
        <div class="container mx-auto px-4 py-4 flex flex-col space-y-4">
            <a href="#home" class="text-dark hover:text-primary transition-custom py-2">首页</a>
            <a href="#about" class="text-dark hover:text-primary transition-custom py-2">关于我们</a>
            <a href="#services" class="text-dark hover:text-primary transition-custom py-2">核心业务</a>
            <a href="#factory" class="text-dark hover:text-primary transition-custom py-2">工厂实景</a>
            <a href="#equipment" class="text-dark hover:text-primary transition-custom py-2">生产设备</a>
            <a href="#series" class="text-dark hover:text-primary transition-custom py-2">适配车型</a>
            <a href="#products" class="text-dark hover:text-primary transition-custom py-2">产品展示</a>
            <a href="#contact" class="text-dark hover:text-primary transition-custom py-2">联系我们</a>
        </div>
    </div>
</nav>

<!-- 首页banner -->
<section id="home" class="relative h-screen flex items-center justify-center bg-cover bg-center" style="background-image: url('https://picsum.photos/id/1071/1920/1080');">
    <div class="absolute inset-0 bg-dark/70"></div>
    <div class="container mx-auto px-4 md:px-8 relative z-10 text-center">
        <h1 class="text-[clamp(2.5rem,5vw,4rem)] font-bold text-white mb-6 leading-tight text-shadow">
            欧克汽车零部件 <span class="text-secondary">品质铸就未来</span>
        </h1>
        <p class="text-[clamp(1rem,2vw,1.25rem)] text-white/90 mb-8 max-w-2xl mx-auto">
            专业的汽车零部件生产企业，集研发、生产、销售、国际贸易于一体，为全球客户提供优质的汽车电子解决方案
        </p>
        <div class="flex flex-col sm:flex-row justify-center gap-4">
            <a href="#contact" class="bg-primary hover:bg-primary/90 text-white font-medium py-3 px-8 rounded-lg transition-custom">立即咨询</a>
            <a href="#products" class="bg-transparent border-2 border-white hover:border-secondary hover:text-secondary text-white font-medium py-3 px-8 rounded-lg transition-custom">查看产品</a>
        </div>
    </div>
    <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 text-white animate-bounce">
        <i class="fa-solid fa-chevron-down text-2xl"></i>
    </div>
</section>

<!-- 关于我们 -->
<section id="about" class="py-20 bg-light">
    <div class="container mx-auto px-4 md:px-8">
        <div class="text-center mb-16">
            <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold mb-4">关于我们</h2>
            <div class="w-20 h-1 bg-primary mx-auto mb-6"></div>
            <p class="text-gray-600 max-w-3xl mx-auto">专业的汽车零部件生产企业，集研发、生产、销售、国际贸易于一体</p>
        </div>
        <div class="grid md:grid-cols-2 gap-12 items-center">
            <div>
                <!-- 公司简介图片 -->
                <img src="https://s41.ax1x.com/2026/03/21/pen00rq.png" alt="厂区" class="rounded-lg shadow-lg w-full h-auto">
            </div>
            <div>
                <h3 class="text-xl font-semibold mb-4 text-primary">公司简介</h3>
                <p class="text-gray-700 mb-6 leading-relaxed">郑州欧克汽车零部件有限公司拥有专业化技术团队，先进的检测设备，完善的生产工艺及一体化生产流程，通过汽车零部件的检测研发，为国内外客商提供优质的附加服务。</p>
                <p class="text-gray-700 mb-6 leading-relaxed">公司集产品销售(汽油、柴油、变速箱、新能源电脑板全系(零售/批发/代发/来样定制)，生产(生产配套方案设计开发、OEM代工代料生产、电子元器件配套采购PCB制作、SMT贴片加工、DIP插件组装测试等)，研发(模块研修、解决汽车电脑模块软硬件问题、在线编程、匹配防盗数据制作、故障诊断、电脑维修精修等)、国际贸易于一体。</p>
                <a href="#contact" class="inline-block mt-4 bg-primary hover:bg-primary/90 text-white font-medium py-2 px-6 rounded-lg transition-custom">联系我们</a>
            </div>
        </div>
    </div>
</section>

<!-- 核心业务 -->
<section id="services" class="py-20 bg-white">
    <div class="container mx-auto px-4 md:px-8">
        <div class="text-center mb-16">
            <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold mb-4">核心业务</h2>
            <div class="w-20 h-1 bg-primary mx-auto mb-6"></div>
            <p class="text-gray-600 max-w-3xl mx-auto">全方位的汽车电子解决方案，覆盖研发、生产、销售全流程</p>
        </div>
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="bg-light rounded-lg p-8 shadow-md hover:shadow-xl">
                <div class="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mb-6">
                    <i class="fa-solid fa-store text-2xl text-primary"></i>
                </div>
                <h3 class="text-xl font-semibold mb-4">产品销售</h3>
                <p class="text-gray-600">汽油、柴油、变速箱、新能源电脑板全系销售，支持零售、批发、代发、来样定制。</p>
            </div>
            <div class="bg-light rounded-lg p-8 shadow-md hover:shadow-xl">
                <div class="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mb-6">
                    <i class="fa-solid fa-industry text-2xl text-primary"></i>
                </div>
                <h3 class="text-xl font-semibold mb-4">生产制造</h3>
                <p class="text-gray-600">OEM代工、SMT贴片、插件测试、电子元器件配套生产。</p>
            </div>
            <div class="bg-light rounded-lg p-8 shadow-md hover:shadow-xl">
                <div class="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mb-6">
                    <i class="fa-solid fa-flask-vial text-2xl text-primary"></i>
                </div>
                <h3 class="text-xl font-semibold mb-4">研发维修</h3>
                <p class="text-gray-600">模块维修、在线编程、防盗匹配、故障诊断、数据制作。</p>
            </div>
        </div>
    </div>
</section>

<!-- 工厂实景 -->
<section id="factory" class="py-20 bg-white">
    <div class="container mx-auto px-4 md:px-8">
        <div class="text-center mb-16">
            <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold mb-4">工厂实景</h2>
            <div class="w-20 h-1 bg-primary mx-auto mb-6"></div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mb-12">
            <!-- 1 物料配套作业区 -->
            <div class="factory-card">
                <img src="https://s41.ax1x.com/2026/03/21/penD7gH.png" alt="物料配套作业区" class="factory-img">
                <div class="p-4 text-center">
                    <h3 class="text-lg font-semibold">物料配套作业区</h3>
                </div>
            </div>
            <!-- 2 SMT车间 -->
            <div class="factory-card">
                <img src="https://s41.ax1x.com/2026/03/21/penDHvd.png" alt="SMT车间" class="factory-img">
                <div class="p-4 text-center">
                    <h3 class="text-lg font-semibold">SMT车间</h3>
                </div>
            </div>
            <!-- 3 AIO车间 -->
            <div class="factory-card">
                <img src="https://s41.ax1x.com/2026/03/21/penDObt.png" alt="AIO车间" class="factory-img">
                <div class="p-4 text-center">
                    <h3 class="text-lg font-semibold">AIO车间</h3>
                </div>
            </div>
            <!-- 4 三防车间 -->
            <div class="factory-card">
                <img src="https://s41.ax1x.com/2026/03/21/penDjVP.jpg" alt="三防车间" class="factory-img">
                <div class="p-4 text-center">
                    <h3 class="text-lg font-semibold">三防车间</h3>
                </div>
            </div>
            <!-- 5 装配车间 -->
            <div class="factory-card">
                <img src="https://s41.ax1x.com/2026/03/21/penDvUf.jpg" alt="装配车间" class="factory-img">
                <div class="p-4 text-center">
                    <h3 class="text-lg font-semibold">装配车间</h3>
                </div>
            </div>
            <!-- 6 功能测试 -->
            <div class="factory-card">
                <img src="https://s41.ax1x.com/2026/03/21/penDx58.png" alt="功能测试" class="factory-img">
                <div class="p-4 text-center">
                    <h3 class="text-lg font-semibold">功能测试</h3>
                </div>
            </div>
        </div>

        <div class="bg-white p-6 rounded-lg shadow-md">
            <p class="text-gray-700 leading-relaxed mb-4">
                郑州欧克拥有专业的采购团队，为多家客户提供PCBA到成品装配代工代料(阻容、二三板管、集成电路、晶版、电感、接插件、PCB、塑胶、五金等)。公司与多家电子元件工厂和代理商建立有长期稳定的合作关系:具备良好的供货周期和供成本优势:减少客户在研发阶段的采购成本及采购时间，严格的供应商稽核管理体系和IQC来料检验，恒温恒湿、ESD静电防护、先进先出管理，确保供应链源流品质
            </p>
            <p class="text-gray-600 text-sm leading-relaxed italic">
                Zhengzhou Ouke has a professional purchasing team, providing PCBA to finished product assembly OEM and component sourcing services (resistors, capacitors, diodes, triodes, integrated circuits, crystal oscillators, inductors, connectors, PCBs, plastics, hardware, etc.) for multiple customers. The company has established long-term and stable cooperative relationships with many electronic component factories and agents: it has advantages in good delivery cycles and supply costs; reduces customers' purchasing costs and time during the R&D stage; implements strict supplier audit management systems and IQC incoming inspection, constant temperature and humidity, ESD electrostatic protection, and FIFO management to ensure the quality of the supply chain from the source.
            </p>
        </div>
    </div>
</section>

<!-- 生产检测设备 -->
<section id="equipment" class="py-20 bg-light">
    <div class="container mx-auto px-4 md:px-8">
        <div class="text-center mb-16">
            <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold mb-4">生产检测设备</h2>
            <div class="w-20 h-1 bg-primary mx-auto mb-6"></div>
            <p class="text-gray-600 max-w-3xl mx-auto">先进的生产检测设备，确保产品品质稳定可靠</p>
        </div>
        <div class="grid md:grid-cols-2 gap-8">
            <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                <img src="https://s41.ax1x.com/2026/03/19/pemm8C4.png" class="w-full h-64 object-cover" alt="国产车防盗匹配平台">
                <div class="p-6"><h3 class="text-xl font-semibold">国产车防盗匹配平台</h3></div>
            </div>
            <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                <img src="https://s41.ax1x.com/2026/03/19/pemmG8J.png" class="w-full h-64 object-cover" alt="ECU综合测试平台">
                <div class="p-6"><h3 class="text-xl font-semibold">ECU综合测试平台</h3></div>
            </div>
        </div>
    </div>
</section>

<!-- 适配车型 -->
<section id="series" class="py-20 bg-white">
    <div class="container mx-auto px-4 md:px-8">
        <div class="text-center mb-16">
            <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold mb-4">适配车型</h2>
            <div class="w-20 h-1 bg-primary mx-auto mb-6"></div>
        </div>
        <div class="grid md:grid-cols-2 gap-8">
            <div class="bg-light p-6 rounded-lg shadow-md h-full">
                <h3 class="text-xl font-semibold text-center mb-4 text-primary">ECU 电脑系列</h3>
                <div class="grid grid-cols-2 sm:grid-cols-3 gap-2">
                    <div class="ecu-tag">M7</div>
                    <div class="ecu-tag">M797</div>
                    <div class="ecu-tag">ME7</div>
                    <div class="ecu-tag">ME17</div>
                    <div class="ecu-tag">ECU6.1</div>
                    <div class="ecu-tag">MG1UA008</div>
                    <div class="ecu-tag">MG1US00/S028</div>
                    <div class="ecu-tag">MG1US708</div>
                    <div class="ecu-tag">MG1US018</div>
                    <div class="ecu-tag">MED17</div>
                    <div class="ecu-tag">ME7.4.4/ME7.4.5</div>
                    <div class="ecu-tag">Cruze</div>
                    <div class="ecu-tag">Continental</div>
                    <div class="ecu-tag">MED17.5.25</div>
                    <div class="ecu-tag">EDC16C39</div>
                    <div class="ecu-tag">EDC17C53</div>
                    <div class="ecu-tag">EDC17C55</div>
                    <div class="ecu-tag">EDC17C63</div>
                    <div class="ecu-tag">EDC17C81</div>
                    <div class="ecu-tag">EDC17C04</div>
                    <div class="ecu-tag">ME17.9.11</div>
                    <div class="ecu-tag">ME17.9.11.1</div>
                    <div class="ecu-tag">ME17.9.21.1</div>
                    <div class="ecu-tag">ME17.9.5</div>
                    <div class="ecu-tag">M7.9.8</div>
                    <div class="ecu-tag">MG7.9.8</div>
                    <div class="ecu-tag">ME17.9.8</div>
                    <div class="ecu-tag">MED17.9.8</div>
                    <div class="ecu-tag">MEG17.9.8</div>
                    <div class="ecu-tag">MEG17.9.12/9.12.1</div>
                    <div class="ecu-tag">MEG17.9.13</div>
                    <div class="ecu-tag">MEG17.9.21</div>
                    <div class="ecu-tag">MT20/20U/20U2/22U</div>
                    <div class="ecu-tag">MT22.1</div>
                    <div class="ecu-tag">MT22.3</div>
                    <div class="ecu-tag">MT60.1</div>
                    <div class="ecu-tag">MT60</div>
                    <div class="ecu-tag">MT62.1/62.1U</div>
                    <div class="ecu-tag">MT62.3</div>
                    <div class="ecu-tag">MT80</div>
                    <div class="ecu-tag">MT92</div>
                    <div class="ecu-tag">MT34</div>
                    <div class="ecu-tag">MTO5</div>
                    <div class="ecu-tag">等系列</div>
                </div>
            </div>

            <div class="bg-light p-6 rounded-lg shadow-md h-full">
                <h3 class="text-xl font-semibold text-center mb-4 text-primary">Vehicle Brand</h3>
                <div class="grid grid-cols-2 sm:grid-cols-3 gap-2">
                    <div class="brand-tag">奔驰/Mercedes-E</div>
                    <div class="brand-tag">宝马/BWM</div>
                    <div class="brand-tag">奥迪/audi</div>
                    <div class="brand-tag">长安/ChangAn</div>
                    <div class="brand-tag">长城/GWM</div>
                    <div class="brand-tag">五菱/WuLing</div>
                    <div class="brand-tag">北汽/BAIC</div>
                    <div class="brand-tag">东风/DFM</div>
                    <div class="brand-tag">众泰/ZOTYE</div>
                    <div class="brand-tag">比亚迪/BYD</div>
                    <div class="brand-tag">吉利/Geely</div>
                    <div class="brand-tag">奇瑞/CHERY</div>
                    <div class="brand-tag">金杯/JinBei</div>
                    <div class="brand-tag">江淮/JAC</div>
                    <div class="brand-tag">力帆/LIFAN</div>
                    <div class="brand-tag">陆风/Landwind</div>
                    <div class="brand-tag">上汽/SAIC</div>
                    <div class="brand-tag">广汽/GAC</div>
                    <div class="brand-tag">一汽/FAW</div>
                    <div class="brand-tag">英朗/Excelle</div>
                    <div class="brand-tag">现代/HYUNDAI</div>
                    <div class="brand-tag">福迪/FODAY</div>
                    <div class="brand-tag">福田/Foton</div>
                    <div class="brand-tag">庆铃/Qingling</div>
                    <div class="brand-tag">黄海/Hanghai</div>
                    <div class="brand-tag">江铃/JMC</div>
                    <div class="brand-tag">等车型</div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- 产品展示 -->
<section id="products" class="py-20 bg-light">
    <div class="container mx-auto px-4 md:px-8">
        <div class="text-center mb-16">
            <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold mb-4">产品展示</h2>
            <div class="w-20 h-1 bg-primary mx-auto mb-6"></div>
        </div>

        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-6">
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjtfg.png" alt="产品展示1" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjYtS.png" alt="产品展示2" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZj30P.png" alt="产品展示3" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZj1mt.png" alt="产品展示4" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjM6A.png" alt="产品展示5" class="w-full h-auto object-contain rounded-md">
            </div>

            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMTVP.png" alt="产品展示6" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMIbt.png" alt="产品展示7" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeM4KA.png" alt="产品展示8" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMWgH.png" alt="产品展示9" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeM2CD.png" alt="产品展示10" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x the 2026/03/18/peeM6UK.png" alt="产品展示11" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMyE6.png" alt="产品展示12" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMrHx.png" alt="产品展示13" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjJk8.png" alt="产品展示14" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZj8Tf.png" alt="产品展示15" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjQOI.png" alt="产品展示16" class="w-full h-auto object-contain rounded-md">
            </div>

            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemm7xs.jpg" alt="产品展示17" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmT2j.jpg" alt="产品展示18" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemm4IS.png" alt="产品展示19" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmha8.jpg" alt="产品展示20" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmfVf.png" alt="产品展示21" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmRqP.png" alt="产品展示22" class="w-full h-auto object-contain rounded-md">
            </div>

            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/peniSpt.png" alt="产品展示23" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penSYVA.png" alt="产品展示24" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penStUI.png" alt="产品展示25" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penS3Ke.png" alt="产品展示26" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penS8DH.png" alt="产品展示27" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penSGbd.png" alt="产品展示28" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penPxfI.jpg" alt="产品展示29" class="w-full h-auto object-contain rounded-md">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penSlvD.jpg" alt="产品展示30" class="w-full h-auto object-contain rounded-md">
            </div>
        </div>
    </div>
</section>

<!-- 联系我们 -->
<section id="contact" class="py-20 bg-light">
    <div class="container mx-auto px-4 md:px-8">
        <div class="text-center mb-16">
            <h2 class="text-[clamp(1.8rem,3vw,2.5rem)] font-bold mb-4">联系我们</h2>
            <div class="w-20 h-1 bg-primary mx-auto mb-6"></div>
        </div>
        <div class="max-w-5xl mx-auto grid md:grid-cols-2 gap-8">
            <div class="bg-white p-8 rounded-lg shadow-md">
                <ul class="space-y-6">
                    <li class="flex items-start">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mr-4">
                            <i class="fa-solid fa-map-marker text-primary"></i>
                        </div>
                        <div>
                            <h4 class="font-medium">公司地址</h4>
                            <p class="text-gray-600">河南省郑州市管城回族区经济技术开发区第二十三大街中科智谷产业园2号楼</p>
                        </div>
                    </li>
                    <li class="flex items-start">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mr-4">
                            <i class="fa-solid fa-phone text-primary"></i>
                        </div>
                        <div>
                            <h4 class="font-medium">联系电话</h4>
                            <p class="text-gray-600">19128796896 / 19120698329</p>
                        </div>
                    </li>
                    <li class="flex items-start">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mr-4">
                            <i class="fa-brands fa-weixin text-primary"></i>
                        </div>
                        <div>
                            <h4 class="font-medium">微信咨询</h4>
                            <p class="text-gray-600">19128796896（微信同号）</p>
                            <p class="text-gray-600 mt-1">扫码添加，支持产品咨询/报价/定制</p>
                        </div>
                    </li>
                </ul>
            </div>
            
            <div class="qrcode-box flex flex-col items-center justify-center">
                <h3 class="text-lg font-semibold mb-4">微信扫码咨询</h3>
                <!-- 已更换为新的微信二维码 -->
                <img src="https://s41.ax1x.com/2026/03/21/penrnGF.png" alt="微信二维码" class="w-60 h-60 rounded-lg shadow-sm">
                <p class="mt-3 text-gray-600">批发/维修/定制/报价 一站式服务</p>
            </div>
        </div>
    </div>
</section>

<footer class="bg-dark text-white pt-16 pb-8">
    <div class="container mx-auto px-4">
        <p class="text-center text-gray-400">© 2026 郑州欧克汽车零部件有限公司版权所有</p>
    </div>
</footer>

<script>
    // 导航栏滚动效果
    const navbar = document.getElementById('navbar');
    window.addEventListener('scroll',()=>{
        navbar.classList.toggle('bg-dark/95 shadow-lg py-2', window.scrollY>50);
    });

    // 移动端菜单切换
    const menuBtn = document.getElementById('menuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    menuBtn.onclick = ()=>{
        mobileMenu.classList.toggle('hidden');
        let i = menuBtn.querySelector('i');
        i.classList.toggle('fa-bars');
        i.classList.toggle('fa-times');
    };
</script>
</body>
</html>
