<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>郑州欧克汽车零部件有限公司-汽车零部件制造商</title>
    <!-- 稳定的 Tailwind CSS CDN 官方最新版 -->
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
                    screens: {
                        'sm': '640px',
                        'md': '768px',
                        'lg': '1024px',
                        'xl': '1280px',
                        '2xl': '1536px',
                        '3xl': '1920px',
                    }
                }
            }
        }
    </script>
    
    <style>
        /* 核心修复：全局样式 100%生效，不依赖Tailwind层级 */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        html { 
            scroll-behavior: smooth; 
            scroll-padding-top: 80px; 
        }
        body {
            font-family: 'Inter', system-ui, sans-serif;
            color: #1D3557;
            background-color: #F1FAEE;
            padding-top: 80px;
            overflow-x: hidden;
        }
        /* 核心修复：全屏宽容器，替代container，确保所有屏幕生效 */
        .wide-container {
            width: 100%;
            margin-left: auto;
            margin-right: auto;
            padding-left: 16px;
            padding-right: 16px;
        }
        @media (min-width: 640px) {
            .wide-container {
                padding-left: 32px;
                padding-right: 32px;
            }
        }
        @media (min-width: 1024px) {
            .wide-container {
                padding-left: 48px;
                padding-right: 48px;
            }
        }
        @media (min-width: 1536px) {
            .wide-container {
                padding-left: 80px;
                padding-right: 80px;
            }
        }

        /* 组件样式，不依赖Tailwind @layer，确保线上生效 */
        .transition-custom {
            transition: all 0.3s ease-in-out;
        }
        .text-shadow {
            text-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        .product-card {
            background: #fff;
            border-radius: 0.5rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease-in-out;
            padding: 1rem;
            border: 1px solid #f3f4f6;
        }
        .product-card:hover {
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .brand-tag {
            background: #fff;
            border-radius: 0.5rem;
            box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
            padding: 0.75rem;
            text-align: center;
            transition: all 0.3s ease-in-out;
            border: 1px solid #f3f4f6;
        }
        .brand-tag:hover {
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            background: rgba(230, 57, 70, 0.05);
        }
        .ecu-tag {
            background: #fff;
            border-radius: 0.375rem;
            padding: 0.5rem;
            text-align: center;
            border: 1px solid #e5e7eb;
            font-size: 0.875rem;
            transition: all 0.3s ease-in-out;
        }
        .ecu-tag:hover {
            background: rgba(230, 57, 70, 0.05);
        }
        .factory-card {
            background: #fff;
            border-radius: 0.5rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: all 0.3s ease-in-out;
        }
        .factory-card:hover {
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .factory-img {
            width: 100%;
            height: auto;
            aspect-ratio: 4/3;
            object-fit: cover;
        }
        .equipment-card {
            background: #fff;
            border-radius: 0.5rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            transition: all 0.3s ease-in-out;
        }
        .equipment-card:hover {
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .equipment-img {
            width: 100%;
            height: 16rem;
            object-fit: cover;
        }
        .qrcode-box {
            background: #fff;
            padding: 1rem;
            border-radius: 0.5rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .image-modal {
            position: fixed;
            inset: 0;
            background: rgba(0, 0, 0, 0.95);
            z-index: 99999;
            display: none;
            align-items: center;
            justify-content: center;
        }
        .close-btn {
            position: absolute;
            top: 1rem;
            right: 1rem;
            color: #fff;
            font-size: 2.5rem;
            cursor: pointer;
            transition: all 0.3s ease-in-out;
            z-index: 100000;
        }
        .close-btn:hover {
            color: #E63946;
        }
    </style>
</head>
<body>

<!-- 导航栏 - 固定顶部，层级最高 -->
<nav id="navbar" style="position: fixed; top: 0; left: 0; width: 100%; z-index: 9999; transition: all 0.3s ease-in-out; padding: 1rem 0; background: #1D3557; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);">
    <div class="wide-container" style="display: flex; justify-content: space-between; align-items: center; width: 100%;">
        <a href="#" style="font-size: 1.5rem; font-weight: 700; color: #fff; text-shadow: 0 2px 4px rgba(0,0,0,0.1); display: flex; align-items: center; flex-shrink: 0;">
            <!-- 公司LOGO -->
            <img 
                src="https://p9-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/7327111515224dbebc11557709f71446.png~tplv-a9rns2rl98-image.png?lk3s=8e244e95&rcl=20260320162540CE54F6183B0F9F0B5D53&rrcfp=dafada99&x-expires=2090219140&x-signature=SVekwt1q9CEMS9R7vJgPcAIWLdo%3D" 
                alt="欧克汽车零部件LOGO" 
                style="height: 2rem; width: auto; margin-right: 0.5rem; object-fit: contain;"
                loading="eager">
            欧克汽车零部件
        </a>
        <!-- 桌面端导航菜单 -->
        <div style="display: none; align-items: center; gap: 2rem;" class="md:flex">
            <a href="#home" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">首页</a>
            <a href="#about" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">关于我们</a>
            <a href="#services" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">核心业务</a>
            <a href="#factory" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">工厂实景</a>
            <a href="#equipment" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">生产设备</a>
            <a href="#series" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">适配车型</a>
            <a href="#products" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">产品展示</a>
            <a href="#contact" style="color: #fff; transition: all 0.3s ease-in-out; white-space: nowrap;" onmouseover="this.style.color='#457B9D'" onmouseout="this.style.color='#fff'">联系我们</a>
        </div>
        <button id="menuBtn" style="display: block; color: #fff; font-size: 1.5rem; flex-shrink: 0;" class="md:hidden">
            <i class="fa-solid fa-bars"></i>
        </button>
    </div>
    <!-- 移动端菜单 -->
    <div id="mobileMenu" style="display: none; background: #fff; box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1); position: absolute; width: 100%; left: 0;" class="md:hidden">
        <div class="wide-container" style="padding: 1rem 16px; display: flex; flex-direction: column; gap: 1rem;">
            <a href="#home" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">首页</a>
            <a href="#about" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">关于我们</a>
            <a href="#services" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">核心业务</a>
            <a href="#factory" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">工厂实景</a>
            <a href="#equipment" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">生产设备</a>
            <a href="#series" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">适配车型</a>
            <a href="#products" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">产品展示</a>
            <a href="#contact" style="color: #1D3557; transition: all 0.3s ease-in-out; padding: 0.5rem 0;" onmouseover="this.style.color='#E63946'" onmouseout="this.style.color='#1D3557'">联系我们</a>
        </div>
    </div>
</nav>

<!-- 首页banner -->
<section id="home" style="position: relative; min-height: calc(100vh - 80px); display: flex; align-items: center; justify-content: center; background-image: url('https://picsum.photos/id/1071/1920/1080'); background-size: cover; background-position: center;">
    <div style="position: absolute; inset: 0; background: rgba(29, 53, 87, 0.7);"></div>
    <div class="wide-container" style="position: relative; z-index: 10; text-align: center;">
        <h1 style="font-size: clamp(2rem, 5vw, 4rem); font-weight: 700; color: #fff; margin-bottom: 1.5rem; line-height: 1.2; text-shadow: 0 2px 4px rgba(0,0,0,0.1);">
            欧克汽车零部件 <span style="color: #457B9D;">品质铸就未来</span>
        </h1>
        <p style="font-size: clamp(1rem, 2vw, 1.25rem); color: rgba(255,255,255,0.9); margin-bottom: 2rem; max-width: 42rem; margin-left: auto; margin-right: auto;">
            专业的汽车零部件生产企业，集研发、生产、销售、国际贸易于一体，为全球客户提供优质的汽车电子解决方案
        </p>
        <div style="display: flex; flex-direction: column; gap: 1rem; justify-content: center;" class="sm:flex-row">
            <a href="#contact" style="background: #E63946; color: #fff; font-weight: 500; padding: 0.75rem 2rem; border-radius: 0.5rem; transition: all 0.3s ease-in-out;" onmouseover="this.style.background='#dc2626'" onmouseout="this.style.background='#E63946'">立即咨询</a>
            <a href="#products" style="background: transparent; border: 2px solid #fff; color: #fff; font-weight: 500; padding: 0.75rem 2rem; border-radius: 0.5rem; transition: all 0.3s ease-in-out;" onmouseover="this.style.borderColor='#457B9D'; this.style.color='#457B9D'" onmouseout="this.style.borderColor='#fff'; this.style.color='#fff'">查看产品</a>
        </div>
    </div>
    <div style="position: absolute; bottom: 2rem; left: 50%; transform: translateX(-50%); color: #fff; animation: bounce 2s infinite;">
        <i class="fa-solid fa-chevron-down" style="font-size: 1.5rem;"></i>
    </div>
</section>

<!-- 核心修复：关于我们板块 100%还原本地效果 -->
<section id="about" style="padding: 4rem 0;" class="md:py-20">
    <div class="wide-container">
        <!-- 关于我们大标题 + 下划线 + 副标题 完全还原本地 -->
        <div style="text-align: center; margin-bottom: 3rem;" class="md:mb-16">
            <h2 style="font-size: clamp(1.8rem, 3vw, 2.5rem); font-weight: 700; margin-bottom: 1rem;">关于我们</h2>
            <div style="width: 5rem; height: 0.25rem; background: #E63946; margin-left: auto; margin-right: auto; margin-bottom: 1.5rem;"></div>
            <p style="color: #4B5563; max-width: 48rem; margin-left: auto; margin-right: auto; font-size: 1.125rem;">
                专业的汽车零部件生产企业，集研发、生产、销售、国际贸易于一体
            </p>
        </div>
        <!-- 左右布局 图片左、文字右 完全还原本地 -->
        <div style="display: grid; gap: 3rem; align-items: center;" class="md:grid-cols-2 md:gap-12">
            <!-- 左侧厂区图片 -->
            <div>
                <img 
                    src="https://s41.ax1x.com/2026/03/21/pen00rq.png" 
                    alt="厂区" 
                    style="border-radius: 0.5rem; box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1); width: 100%; height: auto; object-fit: cover;"
                    loading="lazy">
            </div>
            <!-- 右侧公司简介文字 -->
            <div>
                <h3 style="font-size: 1.25rem; font-weight: 600; margin-bottom: 1rem; color: #E63946;">公司简介</h3>
                <p style="color: #374151; margin-bottom: 1.5rem; line-height: 1.75;">
                    郑州欧克汽车零部件有限公司拥有专业化技术团队，先进的检测设备，完善的生产工艺及一体化生产流程，通过汽车零部件的检测研发，为国内外客商提供优质的附加服务。
                </p>
                <p style="color: #374151; margin-bottom: 1.5rem; line-height: 1.75;">
                    公司集产品销售(汽油、柴油、变速箱、新能源电脑板全系(零售/批发/代发/来样定制)，生产(生产配套方案设计开发、OEM代工代料生产、电子元器件配套采购PCB制作、SMT贴片加工、DIP插件组装测试等)，研发(模块研修、解决汽车电脑模块软硬件问题、在线编程、匹配防盗数据制作、故障诊断、电脑维修精修等)、国际贸易于一体。
                </p>
                <a href="#contact" style="display: inline-block; margin-top: 1rem; background: #E63946; color: #fff; font-weight: 500; padding: 0.5rem 1.5rem; border-radius: 0.5rem; transition: all 0.3s ease-in-out;" onmouseover="this.style.background='#dc2626'" onmouseout="this.style.background='#E63946'">联系我们</a>
            </div>
        </div>
    </div>
</section>

<!-- 核心业务 -->
<section id="services" style="padding: 4rem 0; background: #fff;" class="md:py-20">
    <div class="wide-container">
        <div style="text-align: center; margin-bottom: 3rem;" class="md:mb-16">
            <h2 style="font-size: clamp(1.8rem, 3vw, 2.5rem); font-weight: 700; margin-bottom: 1rem;">核心业务</h2>
            <div style="width: 5rem; height: 0.25rem; background: #E63946; margin-left: auto; margin-right: auto; margin-bottom: 1.5rem;"></div>
            <p style="color: #4B5563; max-width: 48rem; margin-left: auto; margin-right: auto;">
                全方位的汽车电子解决方案，覆盖研发、生产、销售全流程
            </p>
        </div>
        <div style="display: grid; gap: 2rem;" class="md:grid-cols-2 lg:grid-cols-3">
            <div style="background: #F1FAEE; border-radius: 0.5rem; padding: 2rem; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1); transition: all 0.3s ease-in-out;" onmouseover="this.style.boxShadow='0 20px 25px -5px rgba(0, 0, 0, 0.1)'" onmouseout="this.style.boxShadow='0 4px 6px -1px rgba(0, 0, 0, 0.1)'">
                <div style="width: 4rem; height: 4rem; background: rgba(230, 57, 70, 0.1); border-radius: 9999px; display: flex; align-items: center; justify-content: center; margin-bottom: 1.5rem;">
                    <i class="fa-solid fa-store" style="font-size: 1.5rem; color: #E63946;"></i>
                </div>
                <h3 style="font-size: 1.25rem; font-weight: 600; margin-bottom: 1rem;">产品销售</h3>
                <p style="color: #4B5563;">汽油、柴油、变速箱、新能源电脑板全系销售，支持零售、批发、代发、来样定制。</p>
            </div>
            <div style="background: #F1FAEE; border-radius: 0.5rem; padding: 2rem; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1); transition: all 0.3s ease-in-out;" onmouseover="this.style.boxShadow='0 20px 25px -5px rgba(0, 0, 0, 0.1)'" onmouseout="this.style.boxShadow='0 4px 6px -1px rgba(0, 0, 0, 0.1)'">
                <div style="width: 4rem; height: 4rem; background: rgba(230, 57, 70, 0.1); border-radius: 9999px; display: flex; align-items: center; justify-content: center; margin-bottom: 1.5rem;">
                    <i class="fa-solid fa-industry" style="font-size: 1.5rem; color: #E63946;"></i>
                </div>
                <h3 style="font-size: 1.25rem; font-weight: 600; margin-bottom: 1rem;">生产制造</h3>
                <p style="color: #4B5563;">OEM代工、SMT贴片、插件测试、电子元器件配套生产。</p>
            </div>
            <div style="background: #F1FAEE; border-radius: 0.5rem; padding: 2rem; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1); transition: all 0.3s ease-in-out;" onmouseover="this.style.boxShadow='0 20px 25px -5px rgba(0, 0, 0, 0.1)'" onmouseout="this.style.boxShadow='0 4px 6px -1px rgba(0, 0, 0, 0.1)'">
                <div style="width: 4rem; height: 4rem; background: rgba(230, 57, 70, 0.1); border-radius: 9999px; display: flex; align-items: center; justify-content: center; margin-bottom: 1.5rem;">
                    <i class="fa-solid fa-flask-vial" style="font-size: 1.5rem; color: #E63946;"></i>
                </div>
                <h3 style="font-size: 1.25rem; font-weight: 600; margin-bottom: 1rem;">研发维修</h3>
                <p style="color: #4B5563;">模块维修、在线编程、防盗匹配、故障诊断、数据制作。</p>
            </div>
        </div>
    </div>
</section>

<!-- 工厂实景 -->
<section id="factory" style="padding: 4rem 0; background: #fff;" class="md:py-20">
    <div class="wide-container">
        <div style="text-align: center; margin-bottom: 3rem;" class="md:mb-16">
            <h2 style="font-size: clamp(1.8rem, 3vw, 2.5rem); font-weight: 700; margin-bottom: 1rem;">工厂实景</h2>
            <div style="width: 5rem; height: 0.25rem; background: #E63946; margin-left: auto; margin-right: auto; margin-bottom: 1.5rem;"></div>
        </div>

        <div style="display: grid; gap: 1.5rem; margin-bottom: 3rem;" class="sm:grid-cols-2 lg:grid-cols-3 md:gap-8">
            <!-- 1 物料配套作业区 -->
            <div class="factory-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penD7gH.png" 
                    alt="物料配套作业区" 
                    class="factory-img"
                    loading="lazy">
                <div style="padding: 1rem; text-align: center;">
                    <h3 style="font-size: 1.125rem; font-weight: 600;">物料配套作业区</h3>
                </div>
            </div>
            <!-- 2 SMT车间 -->
            <div class="factory-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDHvd.png" 
                    alt="SMT车间" 
                    class="factory-img"
                    loading="lazy">
                <div style="padding: 1rem; text-align: center;">
                    <h3 style="font-size: 1.125rem; font-weight: 600;">SMT车间</h3>
                </div>
            </div>
            <!-- 3 AIO车间 -->
            <div class="factory-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDObt.png" 
                    alt="AIO车间" 
                    class="factory-img"
                    loading="lazy">
                <div style="padding: 1rem; text-align: center;">
                    <h3 style="font-size: 1.125rem; font-weight: 600;">AIO车间</h3>
                </div>
            </div>
            <!-- 4 三防车间 -->
            <div class="factory-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDjVP.jpg" 
                    alt="三防车间" 
                    class="factory-img"
                    loading="lazy">
                <div style="padding: 1rem; text-align: center;">
                    <h3 style="font-size: 1.125rem; font-weight: 600;">三防车间</h3>
                </div>
            </div>
            <!-- 5 装配车间 -->
            <div class="factory-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDvUf.jpg" 
                    alt="装配车间" 
                    class="factory-img"
                    loading="lazy">
                <div style="padding: 1rem; text-align: center;">
                    <h3 style="font-size: 1.125rem; font-weight: 600;">装配车间</h3>
                </div>
            </div>
            <!-- 6 功能测试 -->
            <div class="factory-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penDx58.png" 
                    alt="功能测试" 
                    class="factory-img"
                    loading="lazy">
                <div style="padding: 1rem; text-align: center;">
                    <h3 style="font-size: 1.125rem; font-weight: 600;">功能测试</h3>
                </div>
            </div>
        </div>

        <div style="background: #fff; padding: 1.5rem; border-radius: 0.5rem; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);">
            <p style="color: #374151; line-height: 1.75; margin-bottom: 1rem;">
                郑州欧克拥有专业的采购团队，为多家客户提供PCBA到成品装配代工代料(阻容、二三板管、集成电路、晶版、电感、接插件、PCB、塑胶、五金等)。公司与多家电子元件工厂和代理商建立有长期稳定的合作关系:具备良好的供货周期和供成本优势:减少客户在研发阶段的采购成本及采购时间，严格的供应商稽核管理体系和IQC来料检验，恒温恒湿、ESD静电防护、先进先出管理，确保供应链源流品质
            </p>
            <p style="color: #4B5563; font-size: 0.875rem; line-height: 1.75; font-style: italic;">
                Zhengzhou Ouke has a professional purchasing team, providing PCBA to finished product assembly OEM and component sourcing services (resistors, capacitors, diodes, triodes, integrated circuits, crystal oscillators, inductors, connectors, PCBs, plastics, hardware, etc.) for multiple customers. The company has established long-term and stable cooperative relationships with many electronic component factories and agents: it has advantages in good delivery cycles and supply costs; reduces customers' purchasing costs and time during the R&D stage; implements strict supplier audit management systems and IQC incoming inspection, constant temperature and humidity, ESD electrostatic protection, and FIFO management to ensure the quality of the supply chain from the source.
            </p>
        </div>
    </div>
</section>

<!-- 生产检测设备 -->
<section id="equipment" style="padding: 4rem 0; background: #F1FAEE;" class="md:py-20">
    <div class="wide-container">
        <div style="text-align: center; margin-bottom: 3rem;" class="md:mb-16">
            <h2 style="font-size: clamp(1.8rem, 3vw, 2.5rem); font-weight: 700; margin-bottom: 1rem;">生产检测设备</h2>
            <div style="width: 5rem; height: 0.25rem; background: #E63946; margin-left: auto; margin-right: auto; margin-bottom: 1.5rem;"></div>
            <p style="color: #4B5563; max-width: 48rem; margin-left: auto; margin-right: auto;">
                先进的生产检测设备，确保产品品质稳定可靠
            </p>
        </div>
        <div style="display: grid; gap: 2rem;" class="md:grid-cols-2">
            <div class="equipment-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/19/pemm8C4.png" 
                    class="equipment-img" 
                    alt="国产车防盗匹配平台"
                    loading="lazy">
                <div style="padding: 1.5rem;"><h3 style="font-size: 1.25rem; font-weight: 600;">国产车防盗匹配平台</h3></div>
            </div>
            <div class="equipment-card">
                <img 
                    src="https://s41.ax1x.com/2026/03/19/pemmG8J.png" 
                    class="equipment-img" 
                    alt="ECU综合测试平台"
                    loading="lazy">
                <div style="padding: 1.5rem;"><h3 style="font-size: 1.25rem; font-weight: 600;">ECU综合测试平台</h3></div>
            </div>
        </div>
    </div>
</section>

<!-- 适配车型 -->
<section id="series" style="padding: 4rem 0; background: #fff;" class="md:py-20">
    <div class="wide-container">
        <div style="text-align: center; margin-bottom: 3rem;" class="md:mb-16">
            <h2 style="font-size: clamp(1.8rem, 3vw, 2.5rem); font-weight: 700; margin-bottom: 1rem;">适配车型</h2>
            <div style="width: 5rem; height: 0.25rem; background: #E63946; margin-left: auto; margin-right: auto; margin-bottom: 1.5rem;"></div>
        </div>
        <div style="display: grid; gap: 2rem;" class="md:grid-cols-2">
            <div style="background: #F1FAEE; padding: 1.5rem; border-radius: 0.5rem; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1); height: 100%;">
                <h3 style="font-size: 1.25rem; font-weight: 600; text-align: center; margin-bottom: 1rem; color: #E63946;">ECU 电脑系列</h3>
                <div style="display: grid; gap: 0.5rem;" class="grid-cols-2 sm:grid-cols-3">
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

            <div style="background: #F1FAEE; padding: 1.5rem; border-radius: 0.5rem; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1); height: 100%;">
                <h3 style="font-size: 1.25rem; font-weight: 600; text-align: center; margin-bottom: 1rem; color: #E63946;">Vehicle Brand</h3>
                <div style="display: grid; gap: 0.5rem;" class="grid-cols-2 sm:grid-cols-3">
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
<section id="products" style="padding: 4rem 0; background: #F1FAEE;" class="md:py-20">
    <div class="wide-container">
        <div style="text-align: center; margin-bottom: 3rem;" class="md:mb-16">
            <h2 style="font-size: clamp(1.8rem, 3vw, 2.5rem); font-weight: 700; margin-bottom: 1rem;">产品展示</h2>
            <div style="width: 5rem; height: 0.25rem; background: #E63946; margin-left: auto; margin-right: auto; margin-bottom: 1.5rem;"></div>
        </div>

        <div style="display: grid; gap: 1rem;" class="grid-cols-2 sm:grid-cols-3 lg:grid-cols-5 xl:grid-cols-6 md:gap-6">
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjtfg.png" alt="产品展示1" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjYtS.png" alt="产品展示2" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZj30P.png" alt="产品展示3" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZj1mt.png" alt="产品展示4" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjM6A.png" alt="产品展示5" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMTVP.png" alt="产品展示6" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMIbt.png" alt="产品展示7" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeM4KA.png" alt="产品展示8" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMWgH.png" alt="产品展示9" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeM2CD.png" alt="产品展示10" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeM6UK.png" alt="产品展示11" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMyE6.png" alt="产品展示12" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/18/peeMrHx.png" alt="产品展示13" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjJk8.png" alt="产品展示14" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZj8Tf.png" alt="产品展示15" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/17/peZjQOI.png" alt="产品展示16" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemm7xs.jpg" alt="产品展示17" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmT2j.jpg" alt="产品展示18" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemm4IS.png" alt="产品展示19" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmha8.jpg" alt="产品展示20" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmfVf.png" alt="产品展示21" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/19/pemmRqP.png" alt="产品展示22" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/peniSpt.png" alt="产品展示23" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penSYVA.png" alt="产品展示24" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penStUI.png" alt="产品展示25" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penS3Ke.png" alt="产品展示26" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penS8DH.png" alt="产品展示27" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penSGbd.png" alt="产品展示28" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penPxfI.jpg" alt="产品展示29" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
            <div class="product-card">
                <img src="https://s41.ax1x.com/2026/03/20/penSlvD.jpg" alt="产品展示30" style="width: 100%; height: auto; object-fit: contain; border-radius: 0.375rem;" loading="lazy">
            </div>
        </div>
    </div>
</section>

<!-- 联系我们 -->
<section id="contact" style="padding: 4rem 0; background: #F1FAEE;" class="md:py-20">
    <div class="wide-container">
        <div style="text-align: center; margin-bottom: 3rem;" class="md:mb-16">
            <h2 style="font-size: clamp(1.8rem, 3vw, 2.5rem); font-weight: 700; margin-bottom: 1rem;">联系我们</h2>
            <div style="width: 5rem; height: 0.25rem; background: #E63946; margin-left: auto; margin-right: auto; margin-bottom: 1.5rem;"></div>
        </div>
        <div style="display: grid; gap: 2rem; max-width: 80rem; margin-left: auto; margin-right: auto;" class="md:grid-cols-2">
            <div style="background: #fff; padding: 2rem; border-radius: 0.5rem; box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);">
                <ul style="display: flex; flex-direction: column; gap: 1.5rem;">
                    <li style="display: flex; align-items: flex-start;">
                        <div style="width: 3rem; height: 3rem; background: rgba(230, 57, 70, 0.1); border-radius: 9999px; display: flex; align-items: center; justify-content: center; margin-right: 1rem; flex-shrink: 0;">
                            <i class="fa-solid fa-map-marker" style="color: #E63946;"></i>
                        </div>
                        <div>
                            <h4 style="font-weight: 500; margin-bottom: 0.25rem;">公司地址</h4>
                            <p style="color: #4B5563;">河南省郑州市管城回族区经济技术开发区第二十三大街中科智谷产业园2号楼</p>
                        </div>
                    </li>
                    <li style="display: flex; align-items: flex-start;">
                        <div style="width: 3rem; height: 3rem; background: rgba(230, 57, 70, 0.1); border-radius: 9999px; display: flex; align-items: center; justify-content: center; margin-right: 1rem; flex-shrink: 0;">
                            <i class="fa-solid fa-phone" style="color: #E63946;"></i>
                        </div>
                        <div>
                            <h4 style="font-weight: 500; margin-bottom: 0.25rem;">联系电话</h4>
                            <p style="color: #4B5563;">19128796896 / 19120698329</p>
                        </div>
                    </li>
                    <li style="display: flex; align-items: flex-start;">
                        <div style="width: 3rem; height: 3rem; background: rgba(230, 57, 70, 0.1); border-radius: 9999px; display: flex; align-items: center; justify-content: center; margin-right: 1rem; flex-shrink: 0;">
                            <i class="fa-brands fa-weixin" style="color: #E63946;"></i>
                        </div>
                        <div>
                            <h4 style="font-weight: 500; margin-bottom: 0.25rem;">微信咨询</h4>
                            <p style="color: #4B5563;">19128796896（微信同号）</p>
                            <p style="color: #4B5563; margin-top: 0.25rem;">扫码添加，支持产品咨询/报价/定制</p>
                        </div>
                    </li>
                </ul>
            </div>
            
            <div class="qrcode-box" style="display: flex; flex-direction: column; align-items: center; justify-content: center;">
                <h3 style="font-size: 1.125rem; font-weight: 600; margin-bottom: 1rem;">微信扫码咨询</h3>
                <img 
                    src="https://s41.ax1x.com/2026/03/21/penrnGF.png" 
                    alt="微信二维码" 
                    style="width: 15rem; height: 15rem; border-radius: 0.5rem; box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05); object-fit: contain;"
                    loading="lazy">
                <p style="margin-top: 0.75rem; color: #4B5563;">批发/维修/定制/报价 一站式服务</p>
            </div>
        </div>
    </div>
</section>

<!-- 页脚 -->
<footer style="background: #1D3557; color: #fff; padding: 3rem 0 2rem 0;">
    <div class="wide-container">
        <p style="text-align: center; color: #9CA3AF;">© 2026 郑州欧克汽车零部件有限公司版权所有</p>
    </div>
</footer>

<!-- 图片放大模态框 -->
<div id="imageModal" class="image-modal">
    <span class="close-btn" onclick="closeModal()">&times;</span>
    <div style="max-width: 80rem; max-height: 95vh; padding: 0.5rem;">
        <img id="modalImage" style="width: 100%; height: auto; max-height: 90vh; object-fit: contain;" src="" alt="放大图片">
    </div>
</div>

<!-- 动画样式 -->
<style>
    @keyframes bounce {
        0%, 100% {
            transform: translateY(0);
        }
        50% {
            transform: translateY(-10px);
        }
    }
</style>

<script>
    // 导航栏滚动效果
    const navbar = document.getElementById('navbar');
    window.addEventListener('scroll',()=>{
        if(window.scrollY > 50) {
            navbar.style.padding = '0.5rem 0';
            navbar.style.boxShadow = '0 10px 15px -3px rgba(0, 0, 0, 0.1)';
        } else {
            navbar.style.padding = '1rem 0';
            navbar.style.boxShadow = '0 4px 6px -1px rgba(0, 0, 0, 0.1)';
        }
    });

    // 移动端菜单切换
    const menuBtn = document.getElementById('menuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    menuBtn.onclick = (e)=>{
        e.stopPropagation();
        if(mobileMenu.style.display === 'block') {
            mobileMenu.style.display = 'none';
            menuBtn.querySelector('i').classList.remove('fa-times');
            menuBtn.querySelector('i').classList.add('fa-bars');
        } else {
            mobileMenu.style.display = 'block';
            menuBtn.querySelector('i').classList.remove('fa-bars');
            menuBtn.querySelector('i').classList.add('fa-times');
        }
    };

    // 点击空白处关闭移动端菜单
    document.addEventListener('click', (e) => {
        if(!menuBtn.contains(e.target) && !mobileMenu.contains(e.target)) {
            mobileMenu.style.display = 'none';
            menuBtn.querySelector('i').classList.remove('fa-times');
            menuBtn.querySelector('i').classList.add('fa-bars');
        }
    });

    // 图片放大模态框功能
    const modal = document.getElementById('imageModal');
    const modalImg = document.getElementById('modalImage');
    const allImages = document.querySelectorAll('.product-card img, .factory-img, .equipment-img');

    allImages.forEach(img => {
        img.style.cursor = 'pointer';
        img.onclick = function() {
            modal.style.display = 'flex';
            modalImg.src = this.src;
            modalImg.alt = this.alt;
        }
    });

    function closeModal() {
        modal.style.display = 'none';
    }

    // 点击模态框空白处关闭
    modal.onclick = function(e) {
        if(e.target === modal) {
            closeModal();
        }
    }

    // 键盘ESC关闭模态框
    document.addEventListener('keydown', (e) => {
        if(e.key === 'Escape' && modal.style.display === 'flex') {
            closeModal();
        }
    });
</script>
</body>
</html>
