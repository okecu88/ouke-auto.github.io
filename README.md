<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8" />
  <title>Ouke Auto - 产品展示</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- Tailwind Play CDN 自定义 config -->
  <script src="https://cdn.tailwindcss.com"></script>
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
            sans: ['Inter', 'PingFang SC', 'Microsoft YaHei', 'system-ui', 'sans-serif'],
          },
        }
      }
    }
  </script>
  <style>
    html { scroll-behavior: smooth; }
    .text-shadow { text-shadow: 0 2px 4px rgba(0,0,0,0.1); }
    /* 下面只保留非 @apply 的简单自定义CSS, @apply一律无效 */
    .navbar-scrolled { background-color: rgba(29,53,87,0.95) !important; box-shadow: 0 2px 4px rgba(0,0,0,0.10)!important; padding-top: .5rem !important; padding-bottom: .5rem !important;}
  </style>
</head>
<body class="bg-light font-sans">

  <!-- 导航栏Demo -->
  <nav class="fixed w-full z-10 transition-all duration-300 ease-in-out bg-dark/85 shadow px-6 py-4">
    <span class="text-xl text-primary font-bold">Ouke Auto</span>
  </nav>
  <div class="h-16"></div>
  
  <!-- 样例产品卡片 -->
  <div class="max-w-4xl mx-auto py-8 px-2">
    <h2 class="text-2xl font-bold text-dark mb-6">产品列表</h2>
    <div class="grid md:grid-cols-3 gap-6">
      <div class="bg-white rounded-lg shadow-md hover:shadow-xl transition-all duration-300 ease-in-out p-4 border border-gray-100 cursor-pointer">
        <img src="https://placehold.co/160x100" class="w-full h-32 object-cover rounded mb-4" alt="产品图示"/>
        <div class="text-lg font-bold mb-2 text-dark">产品A</div>
        <div class="text-secondary mb-2">品牌：<span class="inline-block bg-white rounded-lg shadow-sm px-2 py-1 text-sm border border-gray-100">OUKE</span></div>
        <div class="text-gray-600 mb-3 text-sm">这是产品A的描述...</div>
        <div class="text-xs text-gray-500 text-right italic">ECU 编号：12345</div>
      </div>
      <div class="bg-white rounded-lg shadow-md hover:shadow-xl transition-all duration-300 ease-in-out p-4 border border-gray-100 cursor-pointer">
        <img src="https://placehold.co/160x100" class="w-full h-32 object-cover rounded mb-4" alt="产品图示"/>
        <div class="text-lg font-bold mb-2 text-dark">产品B</div>
        <div class="text-secondary mb-2">品牌：<span class="inline-block bg-white rounded-lg shadow-sm px-2 py-1 text-sm border border-gray-100">OUKE</span></div>
        <div class="text-gray-600 mb-3 text-sm">这是产品B的描述...</div>
        <div class="text-xs text-gray-500 text-right italic">ECU 编号：67890</div>
      </div>
      <div class="bg-white rounded-lg shadow-md hover:shadow-xl transition-all duration-300 ease-in-out p-4 border border-gray-100 cursor-pointer">
        <img src="https://placehold.co/160x100" class="w-full h-32 object-cover rounded mb-4" alt="产品图示"/>
        <div class="text-lg font-bold mb-2 text-dark">产品C</div>
        <div class="text-secondary mb-2">品牌：<span class="inline-block bg-white rounded-lg shadow-sm px-2 py-1 text-sm border border-gray-100">OUKE</span></div>
        <div class="text-gray-600 mb-3 text-sm">这是产品C的描述...</div>
        <div class="text-xs text-gray-500 text-right italic">ECU 编号：54321</div>
      </div>
    </div>
    <!-- 二维码区域DEMO -->
    <div class="mt-10 max-w-sm mx-auto bg-white p-4 rounded-lg shadow-md text-center">
      <div class="mb-4 font-semibold">关注我们的微信：</div>
      <img src="https://placehold.co/100x100?text=QR" alt="微信二维码" class="mx-auto mb-2" />
      <div class="text-gray-500 text-xs">扫码关注获取更多资讯</div>
    </div>
  </div>

</body>
</html>
