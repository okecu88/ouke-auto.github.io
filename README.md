<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>郑州欧克汽车零部件有限公司</title>
    <!-- 官方稳定Tailwind CDN，确保GitHub Pages正常加载 -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- 稳定的字体图标CDN -->
    <link rel="stylesheet" href="https://cdn.bootcdn.net/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <!-- 核心配置：颜色、断点适配GitHub Pages全屏幕 -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#E63946',
                        secondary: '#457B9D',
                        dark: '#1E3A5F',
                        light: '#F0F9F0',
                        card: '#F0F9F0',
                    },
                    fontFamily: {
                        sans: ['system-ui', 'sans-serif'],
                    },
                    screens: {
                        'sm': '640px',
                        'md': '768px',
                        'lg': '1024px',
                        'xl': '1280px',
                        '2xl': '1536px',
                    }
                }
            }
        }
    </script>

    <!-- 全局核心样式：原生CSS编写，避免Tailwind加载异常，确保GitHub Pages100%生效 -->
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        html {
            scroll-behavior: smooth;
            scroll-padding-top: 80px; /* 适配固定导航栏，锚点跳转不被遮挡 */
        }
        body {
            font-family: system-ui, sans-serif;
            background-color: #F0F9F0;
            color: #1E3A5F;
            padding-top: 80px; /* 固定导航栏不遮挡内容 */
            overflow-x: hidden;
            line-height: 1.6;
        }
        /* 全屏容器，适配所有屏幕，GitHub Pages无宽度限制 */
        .page-container {
            width: 100%;
            max-width: 100%;
            padding-left: 1.5rem;
            padding-right: 1.5rem;
            margin-left: auto;
            margin-right: auto;
        }
        @media (min-width: 1024px) {
            .page-container {
                padding-left: 3rem;
                padding-right: 3rem;
            }
        }
        @media (min-width: 1536px) {
            .page-container {
                padding-left: 5rem;
                padding-right: 5rem;
            }
        }
        /* 模块标题统一样式，和本地效果完全一致 */
        .section-title {
            font-size: clamp(1.8rem, 4vw, 2.5rem);
            font-weight: 700;
            text-align: center;
            color: #1E3A5F;
            margin-bottom: 0.75rem;
        }
        .section-line {
            width: 5rem;
            height: 0.25rem;
            background-color: #E63946;
            margin-left: auto;
            margin-right: auto;
            margin-bottom: 1.5rem;
        }
        .section-desc {
            text-align: center;
            color: #374151;
            font-size: 1.125rem;
            max-width: 50rem;
            margin-left: auto;
            margin-right: auto;
            margin-bottom: 3rem;
        }
        /* 卡片统一样式，和本地圆角、阴影完全一致 */
        .base-card {
            background-color: #fff;
            border-radius: 0.75rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: all 0.3s ease;
        }
        .base-card:hover {
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .light-card {
            background-color: #F0F9F0;
            border-radius: 0.75rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
        }
        .light-card:hover {
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        /* 导航栏固定样式 */
        #navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 9999;
            background-color: #1E3A5F;
            padding: 1rem 0;
            transition: all 0.3s ease;
        }
        /* 图片自适应 */
        .img-auto {
            width: 100%;
            height: auto;
            object-fit: cover;
        }
        /* 动画 */
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
    </style>
</head>
<body>

<!-- 导航栏：固定顶部，和本地效果完全一致，GitHub Pages无错位 -->
<nav id="navbar">
    <div class="page-container flex justify-between items-center">
        <!-- LOGO+公司名称 -->
        <a href="#home" class="flex items-center text-white font-bold text-2xl">
            <img 
                src="https://p9-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/7327111515224dbebc11557709f71446.png~tplv-a9rns2rl98-image.png" 
                alt="欧克汽车零部件LOGO" 
                class="h-10 w-auto mr-3 object-contain"
                loading="eager">
            欧克汽车零部件
        </a>

        <!-- 桌面端导航菜单 -->
        <div class="hidden md:flex items-center space-x-6 lg:space-x-8">
            <a href="#home" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">首页</a>
            <a href="#about" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">关于我们</a>
            <a href="#services" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">核心业务</a>
            <a href="#factory" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">工厂实景</a>
            <a href="#equipment" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">生产设备</a>
            <a href="#series" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">适配车型</a>
            <a href="#products" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">产品展示</a>
            <a href="#contact" class="text-white hover:text-gray-200 transition-all text-lg whitespace-nowrap">联系我们</a>
        </div>

        <!-- 移动端汉堡菜单 -->
        <button id="menuBtn" class="md:hidden text-white text-2xl">
            <i class="fa-solid fa-bars"></i>
        </button>
    </div>

    <!-- 移动端下拉菜单 -->
    <div id="mobileMenu" class="md:hidden hidden bg-white shadow-lg absolute w-full left-0">
        <div class="page-container py-4 flex flex-col space-y-4">
            <a href="#home" class="text-dark hover:text-primary py-2 text-lg">首页</a>
            <a href="#about" class="text-dark hover:text-primary py-2 text-lg">关于我们</a>
            <a href="#services" class="text-dark hover:text-primary py-2 text-lg">核心业务</a>
            <a href="#factory" class="text-dark hover:text-primary py-2 text-lg">工厂实景</a>
            <a href="#equipment" class="text-dark hover:text-primary py-2 text-lg">生产设备</a>
            <a href="#series" class="text-dark hover:text-primary py-2 text-lg">适配车型</a>
            <a href="#products" class="text-dark hover:text-primary py-2 text-lg">产品展示</a>
            <a href="#contact" class="text-dark hover:text-primary py-2 text-lg">联系我们</a>
        </div>
    </div>
</nav>

<!-- 首页Banner：和本地效果完全一致，全屏高度 -->
<section id="home" class="relative min-h-[calc(100vh-80px)] flex items-center justify-center bg-cover bg-center" style="background-image: url('https://picsum.photos/id/1071/1920/1080');">
    <div class="absolute inset-0 bg-dark/70"></div>
    <div class="page-container relative z-10 text-center">
        <h1 class="text-[clamp(2rem, 6vw, 3.5rem)] font-bold text-white mb-6 leading-tight">
            欧克汽车零部件 <span class="text-secondary">品质铸就未来</span>
        </h1>
        <p class="text-[clamp(1rem, 2vw, 1.25rem)] text-white/95 mb-8 max-w-3xl mx-auto">
            专业的汽车零部件生产企业，集研发、生产、销售、国际贸易于一体，为全球客户提供优质的汽车电子解决方案
        </p>
        <div class="flex flex-col sm:flex-row justify-center gap-4">
            <a href="#contact" class="bg-primary hover:bg-primary/90 text-white font-medium py-3 px-8 rounded-lg text-lg transition-all">立即咨询</a>
            <a href="#products" class="bg-transparent border-2 border-white hover:border-secondary hover:text-secondary text-white font-medium py-3 px-8 rounded-lg text-lg transition-all">查看产品</a>
        </div>
    </div>
    <!-- 向下箭头动画 -->
    <div class="absolute bottom-8 left-1/2 transform -translate-x-1/2 text-white animate-bounce">
        <i class="fa-solid fa-chevron-down text-2xl"></i>
    </div>
</section>

<!-- 关于我们模块：100%还原本地左右布局效果 -->
<section id="about" class="py-16 lg:py-20">
    <div class="page-container">
        <!-- 模块标题 -->
        <h2 class="section-title">关于我们</h2>
        <div class="section-line"></div>
        <p class="section-desc">专业的汽车零部件生产企业，集研发、生产、销售、国际贸易于一体</p>

        <!-- 左右内容区：左图右文 -->
        <div class="grid md:grid-cols-2 gap-8 lg:gap-12 items-center">
            <!-- 左侧厂区图片 -->
            <div>
                <img 
                    src="https://s41.ax1x.com/2026/03/21/pen00rq.png" 
                    alt="厂区实景" 
                    class="img-auto rounded-lg shadow-xl"
                    loading="lazy">
            </div>
            <!-- 右侧公司简介 -->
            <div>
                <h3 class="text-2xl font-semibold mb-4 text-primary">公司简介</h3>
                <p class="text-gray-700 mb-6 text-lg leading-relaxed">
                    郑州欧克汽车零部件有限公司拥有专业化技术团队，先进的检测设备，完善的生产工艺及一体化生产流程，通过汽车零部件的检测研发，为国内外客商提供优质的附加服务。
                </p>
                <p class="text-gray-700 mb-6 text-lg leading-relaxed">
                    公司集产品销售(汽油、柴油、变速箱、新能源电脑板全系(零售/批发/代发/来样定制)，生产(生产配套方案设计开发、OEM代工代料生产、电子元器件配套采购PCB制作、SMT贴片加工、DIP插件组装测试等)，研发(模块研修、解决汽车电脑模块软硬件问题、在线编程、匹配防盗数据制作、故障诊断、电脑维修精修等)、国际贸易于一体。
                </p>
                <a href="#contact" class="inline-block bg-primary hover:bg-primary/90 text-white font-medium py-2.5 px-6 rounded-lg text-lg transition-all">联系我们</a>
            </div>
        </div>
    </div>
</section>

<!-- 核心业务模块：100%还原本地三卡片效果 -->
<section id="services" class="py-16 lg:py-20 bg-white">
    <div class="page-container">
        <h2 class="section-title">核心业务</h2>
        <div class="section-line"></div>
        <p class="section-desc">全方位的汽车电子解决方案，覆盖研发、生产、销售全流程</p>

        <!-- 三个业务卡片 -->
        <div class="grid md:grid-cols-3 gap-8">
            <!-- 产品销售 -->
            <div class="light-card p-8">
                <div class="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mb-6">
                    <i class="fa-solid fa-store text-2xl text-primary"></i>
                </div>
                <h3 class="text-xl font-bold mb-4">产品销售</h3>
                <p class="text-gray-700 text-lg">
                    汽油、柴油、变速箱、新能源电脑板全系销售，支持零售、批发、代发、来样定制。
                </p>
            </div>
            <!-- 生产制造 -->
            <div class="light-card p-8">
                <div class="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mb-6">
                    <i class="fa-solid fa-industry text-2xl text-primary"></i>
                </div>
                <h3 class="text-xl font-bold mb-4">生产制造</h3>
                <p class="text-gray-700 text-lg">
                    OEM代工、SMT贴片、插件测试、电子元器件配套生产。
                </p>
            </div>
            <!-- 研发维修 -->
            <div class="light-card p-8">
                <div class="w-16 h-16 bg-primary/10 rounded-full flex items-center justify-center mb-6">
                    <i class="fa-solid fa-flask-vial text-2xl text-primary"></i>
                </div>
                <h3 class="text-xl font-bold mb-4">研发维修</h3>
                <p class="text-gray-700 text-lg">
                    模块维修、在线编程、防盗匹配、故障诊断、数据制作。
                </p>
            </div>
        </div>
    </div>
</section>

<!-- 工厂实景模块：100%还原本地6图网格效果 -->
<section id="factory" class="py-16 lg:py-20 bg-white">
    <div class="page-container">
        <h2 class="section-title">工厂实景</h2>
        <div class="section-line"></div>

        <!-- 工厂图片网格 -->
        <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- 物料配套作业区 -->
            <div class="base-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penD7gH.png" 
                    alt="物料配套作业区" 
                    class="img-auto h-64"
                    loading="lazy">
                <div class="p-4 text-center">
                    <h3 class="text-xl font-semibold">物料配套作业区</h3>
                </div>
            </div>
            <!-- SMT车间 -->
            <div class="base-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDHvd.png" 
                    alt="SMT车间" 
                    class="img-auto h-64"
                    loading="lazy">
                <div class="p-4 text-center">
                    <h3 class="text-xl font-semibold">SMT车间</h3>
                </div>
            </div>
            <!-- AIO车间 -->
            <div class="base-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDObt.png" 
                    alt="AIO车间" 
                    class="img-auto h-64"
                    loading="lazy">
                <div class="p-4 text-center">
                    <h3 class="text-xl font-semibold">AIO车间</h3>
                </div>
            </div>
            <!-- 三防车间 -->
            <div class="base-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDjVP.jpg" 
                    alt="三防车间" 
                    class="img-auto h-64"
                    loading="lazy">
                <div class="p-4 text-center">
                    <h3 class="text-xl font-semibold">三防车间</h3>
                </div>
            </div>
            <!-- 装配车间 -->
            <div class="base-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDvUf.jpg" 
                    alt="装配车间" 
                    class="img-auto h-64"
                    loading="lazy">
                <div class="p-4 text-center">
                    <h3 class="text-xl font-semibold">装配车间</h3>
                </div>
            </div>
            <!-- 功能测试 -->
            <div class="base-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDx58.png" 
                    alt="功能测试" 
                    class="img-auto h-64"
                    loading="lazy">
                <div class="p-4 text-center">
                    <h3 class="text-xl font-semibold">功能测试</h3>
                </div>
            </div>
        </div>

        <!-- 底部说明文字 -->
        <div class="mt-12 bg-white p-6 rounded-lg shadow-md">
            <p class="text-gray-700 text-lg leading-relaxed">
                郑州欧克拥有专业的采购团队，为多家客户提供PCBA到成品装配代工代料(阻容、二三板管、集成电路、晶版、电感、接插件、PCB、塑胶、五金等)。公司与多家电子元件工厂和代理商建立有长期稳定的合作关系:具备良好的供货周期和供成本优势:减少客户在研发阶段的采购成本及采购时间，严格的供应商稽核管理体系和IQC来料检验，恒温恒湿、ESD静电防护、先进先出管理，确保供应链源流品质
            </p>
            <p class="text-gray-600 text-sm mt-4 leading-relaxed italic">
                Zhengzhou Ouke has a professional purchasing team, providing PCBA to finished product assembly OEM and component sourcing services for multiple customers. The company has established long-term and stable cooperative relationships with many electronic component factories and agents, ensuring the quality of the supply chain from the source.
            </p>
        </div>
    </div>
</section>

<!-- 生产检测设备模块：100%还原本地左右卡片效果 -->
<section id="equipment" class="py-16 lg:py-20">
    <div class="page-container">
        <h2 class="section-title">生产检测设备</h2>
        <div class="section-line"></div>
        <p class="section-desc">先进的生产检测设备，确保产品品质稳定可靠</p>

        <!-- 设备卡片 -->
        <div class="grid md:grid-cols-2 gap-8">
            <!-- 国产车防盗匹配平台 -->
            <div class="base-card">
                <div class="p-6 grid md:grid-cols-2 gap-4 items-center">
                    <div>
                        <ul class="space-y-2 text-gray-700">
                            <li>· 自研LZL-01型国产车防盗线下编程平台，平台内置电源模块及各国产车防盗编程模块，支持国产车防盗类型达到90%，</li>
                            <li>包括防盗盒防盗系统，车身防盗系统，智能一键启动防盗系统。</li>
                            <li>· 线下平台可以配合市面上所有型号的ECU试验台，发动机测试平台使用。</li>
                            <li>· 支持车型全面，线下操作。</li>
                            <li>· 避免车上线路干扰，一次性解决防盗车辆防盗系统问题</li>
                            <li>· 汽车钥匙-汽车仪表-汽车防盗模块-方向锁-网关模块-汽车发动机电脑板组成的防盗系统。</li>
                        </ul>
                        <h3 class="text-xl font-bold mt-6">国产车防盗匹配平台</h3>
                    </div>
                    <div>
                        <img 
                            src="https://s41.ax1x.com/2026/03/19/pemm8C4.png" 
                            alt="国产车防盗匹配平台" 
                            class="img-auto rounded-md"
                            loading="lazy">
                    </div>
                </div>
            </div>
            <!-- ECU综合测试平台 -->
            <div class="base-card">
                <div class="p-6 grid md:grid-cols-2 gap-4 items-center">
                    <div>
                        <ul class="space-y-2 text-gray-700">
                            <li>· 在汽车智能化浪潮席卷全球的今天，ECU作为汽车的“大脑”，其性能直接影响着车辆的操控、安全和效率。</li>
                            <li>郑州欧克汽车零部件有限公司倾力打造汽车ECU智能检测平台，以尖端科技赋能汽车电子诊断，为汽车后市场提供高效、精准、可靠的解决方案</li>
                            <li>· 智能诊断引擎:深度解析ECU数据流，精准定位故障点，提供专业维修建议，大幅提升诊断效率和准确率</li>
                            <li>· 全车型覆盖:支持市面上主流品牌车型的ECU检测，满足不同用户的多样化需求</li>
                            <li>· 云端数据互联:实时更新车型数据库，并支持远程诊断和数据分析，为用户提供更便捷、高效的服务体验</li>
                            <li>· 人性化操作界面:简洁直观的操作界面，即使是非专业人员也能轻松上手，快速掌握ECU检测技能</li>
                        </ul>
                        <h3 class="text-xl font-bold mt-6">ECU综合测试平台</h3>
                    </div>
                    <div>
                        <img 
                            src="https://s41.ax1x.com/2026/03/19/pemmG8J.png" 
                            alt="ECU综合测试平台" 
                            class="img-auto rounded-md"
                            loading="lazy">
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- 适配车型模块：100%还原本地左右两栏标签效果 -->
<section id="series" class="py-16 lg:py-20 bg-white">
    <div class="page-container">
        <div class="grid md:grid-cols-2 gap-8 lg:gap-12">
            <!-- 左侧ECU电脑系列 -->
            <div>
                <h3 class="text-2xl font-bold text-center mb-6 text-primary">ECU 电脑系列</h3>
                <div class="grid grid-cols-3 gap-3">
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">M7</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">M797</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME7</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME17</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ECU6.1</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MG1UA008</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MG1US00/S028</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MG1US708</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MG1US018</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MED17</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME7.4.4/ME7.4.5</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">Cruze</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">Continental</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MED17.5.25</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">EDC16C39</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">EDC17C53</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">EDC17C55</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">EDC17C63</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">EDC17C81</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">EDC17C04</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME17.9.11</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME17.9.11.1</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME17.9.21.1</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME17.9.5</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">M7.9.8</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MG7.9.8</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">ME17.9.8</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MED17.9.8</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MEG17.9.8</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MEG17.9.12/9.12.1</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MEG17.9.13</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MEG17.9.21</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT20/20U/20U2/22U</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT22.1</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT22.3</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT60.1</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT60</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT62.1/62.1U</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT62.3</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT80</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT92</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MT34</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">MTO5</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200 col-span-3">等系列</div>
                </div>
            </div>

            <!-- 右侧车型品牌 -->
            <div>
                <h3 class="text-2xl font-bold text-center mb-6 text-primary">Vehicle Brand</h3>
                <div class="grid grid-cols-3 gap-3">
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">奔驰/Mercedes-E</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">宝马/BWM</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">奥迪/audi</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">长安/ChangAn</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">长城/GWM</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">五菱/WuLing</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">北汽/BAIC</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">东风/DFM</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">众泰/ZOTYE</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">比亚迪/BYD</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">吉利/Geely</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">奇瑞/CHERY</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">金杯/JinBei</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">江淮/JAC</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">力帆/LIFAN</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">陆风/Landwind</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">上汽/SAIC</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">广汽/GAC</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">一汽/FAW</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">英朗/Excelle</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">现代/HYUNDAI</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">福迪/FODAY</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">福田/Foton</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">庆铃/Qingling</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">黄海/Hanghai</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200">江铃/JMC</div>
                    <div class="bg-white rounded-md p-3 text-center border border-gray-200 col-span-3">等车型</div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- 产品展示模块：100%还原本地网格卡片效果 -->
<section id="products" class="py-16 lg:py-20">
    <div class="page-container">
        <h2 class="section-title">产品展示</h2>
        <div class="section-line"></div>

        <!-- 产品网格 -->
        <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 gap-6">
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/17/peZjtfg.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/17/peZjYtS.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/17/peZj30P.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/17/peZj1mt.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/17/peZjM6A.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeMTVP.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeMIbt.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeM4KA.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeMWgH.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeM2CD.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeM6UK.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeMyE6.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/18/peeMrHx.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/17/peZjJk8.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
            <div class="base-card p-4">
                <img src="https://s41.ax1x.com/2026/03/17/peZj8Tf.png" alt="产品" class="img-auto rounded-md" loading="lazy">
            </div>
        </div>
    </div>
</section>

<!-- 联系我们模块：100%还原本地左右卡片效果 -->
<section id="contact" class="py-16 lg:py-20">
    <div class="page-container">
        <h2 class="section-title">联系我们</h2>
        <div class="section-line"></div>

        <div class="grid md:grid-cols-2 gap-8 max-w-6xl mx-auto">
            <!-- 左侧联系信息 -->
            <div class="base-card p-8">
                <ul class="space-y-8">
                    <li class="flex items-start">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mr-4 flex-shrink-0">
                            <i class="fa-solid fa-map-marker text-xl text-primary"></i>
                        </div>
                        <div>
                            <h4 class="text-lg font-semibold mb-1">公司地址</h4>
                            <p class="text-gray-700 text-lg">河南省郑州市管城回族区经济技术开发区第二十三大街中科智谷产业园2号楼</p>
                        </div>
                    </li>
                    <li class="flex items-start">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mr-4 flex-shrink-0">
                            <i class="fa-solid fa-phone text-xl text-primary"></i>
                        </div>
                        <div>
                            <h4 class="text-lg font-semibold mb-1">联系电话</h4>
                            <p class="text-gray-700 text-lg">19128796896 / 19120698329</p>
                        </div>
                    </li>
                    <li class="flex items-start">
                        <div class="w-12 h-12 bg-primary/10 rounded-full flex items-center justify-center mr-4 flex-shrink-0">
                            <i class="fa-brands fa-weixin text-xl text-primary"></i>
                        </div>
                        <div>
                            <h4 class="text-lg font-semibold mb-1">微信咨询</h4>
                            <p class="text-gray-700 text-lg">19128796896（微信同号）</p>
                            <p class="text-gray-600 mt-1">扫码添加，支持产品咨询/报价/定制</p>
                        </div>
                    </li>
                </ul>
            </div>

            <!-- 右侧二维码 -->
            <div class="base-card p-8 flex flex-col items-center justify-center">
                <h3 class="text-xl font-bold mb-4">微信扫码咨询</h3>
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penrnGF.png" 
                    alt="微信二维码" 
                    class="w-60 h-60 object-contain rounded-md"
                    loading="lazy">
                <p class="mt-4 text-gray-700 text-lg">批发/维修/定制/报价 一站式服务</p>
            </div>
        </div>
    </div>
</section>

<!-- 页脚 -->
<footer class="bg-dark text-white py-8">
    <div class="page-container">
        <p class="text-center text-gray-300">© 2026 郑州欧克汽车零部件有限公司版权所有</p>
    </div>
</footer>

<!-- 图片放大查看模态框 -->
<div id="imageModal" class="fixed inset-0 bg-black/95 z-[10000] hidden flex items-center justify-center">
    <span class="absolute top-6 right-6 text-white text-4xl cursor-pointer hover:text-primary" onclick="closeModal()">&times;</span>
    <div class="max-w-6xl max-h-[95vh] p-4">
        <img id="modalImg" class="w-full h-auto max-h-[90vh] object-contain" src="" alt="放大图片">
    </div>
</div>

<!-- 交互JS：确保GitHub Pages正常运行 -->
<script>
    // 导航栏滚动效果
    const navbar = document.getElementById('navbar');
    window.addEventListener('scroll', () => {
        if (window.scrollY > 50) {
            navbar.style.padding = '0.5rem 0';
            navbar.style.boxShadow = '0 10px 15px -3px rgba(0, 0, 0, 0.1)';
        } else {
            navbar.style.padding = '1rem 0';
            navbar.style.boxShadow = 'none';
        }
    });

    // 移动端菜单切换
    const menuBtn = document.getElementById('menuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    menuBtn.addEventListener('click', (e) => {
        e.stopPropagation();
        mobileMenu.classList.toggle('hidden');
        const icon = menuBtn.querySelector('i');
        icon.classList.toggle('fa-bars');
        icon.classList.toggle('fa-times');
    });

    // 点击空白关闭移动端菜单
    document.addEventListener('click', (e) => {
        if (!menuBtn.contains(e.target) && !mobileMenu.contains(e.target)) {
            mobileMenu.classList.add('hidden');
            menuBtn.querySelector('i').classList.remove('fa-times');
            menuBtn.querySelector('i').classList.add('fa-bars');
        }
    });

    // 点击导航链接关闭移动端菜单
    const mobileLinks = mobileMenu.querySelectorAll('a');
    mobileLinks.forEach(link => {
        link.addEventListener('click', () => {
            mobileMenu.classList.add('hidden');
            menuBtn.querySelector('i').classList.remove('fa-times');
            menuBtn.querySelector('i').classList.add('fa-bars');
        });
    });

    // 图片点击放大功能
    const modal = document.getElementById('imageModal');
    const modalImg = document.getElementById('modalImg');
    const allImages = document.querySelectorAll('section img');

    allImages.forEach(img => {
        img.style.cursor = 'pointer';
        img.addEventListener('click', () => {
            modal.style.display = 'flex';
            modalImg.src = img.src;
            modalImg.alt = img.alt;
        });
    });

    // 关闭模态框
    function closeModal() {
        modal.style.display = 'none';
    }

    // 点击模态框空白关闭
    modal.addEventListener('click', (e) => {
        if (e.target === modal) closeModal();
    });

    // ESC键关闭模态框
    document.addEventListener('keydown', (e) => {
        if (e.key === 'Escape' && modal.style.display === 'flex') closeModal();
    });
</script>
</body>
</html>
