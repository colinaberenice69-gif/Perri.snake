<!DOCTYPE html>  
<html lang="es">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>PERRI SNACK | Premios y Productos Orgánicos para Mascotas</title>  
    <!-- Tailwind CSS -->  
    <script src="https://cdn.tailwindcss.com"></script>  
    <!-- FontAwesome Icons -->  
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">  
    <!-- Google Fonts -->  
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">  
    <script>  
        tailwind.config = {  
            theme: {  
                extend: {  
                    colors: {  
                        brand: {  
                            50: '#fdf8f0',  
                            100: '#f9edd8',  
                            200: '#f3d8af',  
                            500: '#e59832',  
                            600: '#d97d20',  
                            700: '#b55e17',  
                            800: '#8f4618',  
                            green: '#4f772d',  
                            greenDark: '#31572c',  
                            bgWarm: '#fefae0'  
                        }  
                    },  
                    fontFamily: {  
                        fredoka: ['Fredoka', 'sans-serif'],  
                        quicksand: ['Quicksand', 'sans-serif']  
                    }  
                }  
            }  
        }  
    </script>  
    <style>  
        body {  
            font-family: 'Quicksand', sans-serif;  
            background-color: #faf7f2;  
        }  
        h1, h2, h3, h4, .font-heading {  
            font-family: 'Fredoka', sans-serif;  
        }  
        .custom-scrollbar::-webkit-scrollbar {  
            width: 6px;  
        }  
        .custom-scrollbar::-webkit-scrollbar-track {  
            background: #f1f1f1;  
            border-radius: 10px;  
        }  
        .custom-scrollbar::-webkit-scrollbar-thumb {  
            background: #d97d20;  
            border-radius: 10px;  
        }  
    </style>  
</head>  
<body class="text-gray-800 flex flex-col min-h-screen">  
  
    <!-- Barra Superior de Contacto Rápido -->  
    <div class="bg-brand-greenDark text-white py-2 px-4 text-xs sm:text-sm font-medium">  
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-2">  
            <div class="flex items-center gap-4">  
                <span><i class="fa-solid fa-phone mr-1.5 text-brand-500"></i> Atencion al Cliente: <a href="tel:+528124129387" class="hover:underline font-bold">+52 (812) 412-9387</a></span>  
                <span class="hidden md:inline">|</span>  
                <span class="hidden md:inline"><i class="fa-solid fa-leaf mr-1.5 text-green-400"></i> Envíos 100% Orgánicos y Libres de Empaque Plástico</span>  
            </div>  
            <div class="flex items-center gap-3">  
                <a href="https://wa.me/528124129387" target="_blank" class="bg-green-600 hover:bg-green-500 text-white px-2.5 py-0.5 rounded-full flex items-center text-xs font-bold transition">  
                    <i class="fa-brands fa-whatsapp mr-1 text-sm"></i> WhatsApp Directo  
                </a>  
                <span class="text-xs text-yellow-300 font-bold">¡Envío Gratis en compras mayores a $499!</span>  
            </div>  
        </div>  
    </div>  
  
    <!-- Navegación Principal -->  
    <header class="bg-white shadow-sm sticky top-0 z-40">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">  
            <!-- Logo -->  
            <a href="#" class="flex items-center gap-3 group">  
                <div class="w-12 h-12 bg-brand-500 text-white rounded-2xl flex items-center justify-center text-2xl shadow-md group-hover:rotate-12 transition-transform duration-300">  
                    <i class="fa-solid fa-bone"></i>  
                </div>  
                <div>  
                    <span class="font-heading text-2xl sm:text-3xl font-bold text-brand-800 tracking-wide block leading-none">PERRI <span class="text-brand-500">SNACK</span></span>  
                    <span class="text-[10px] uppercase font-bold text-brand-green tracking-widest block">Snacks Orgánicos Naturales</span>  
                </div>  
            </a>  
  
            <!-- Enlaces de navegación desktop -->  
            <nav class="hidden md:flex items-center gap-8 font-semibold text-gray-700">  
                <a href="#inicio" class="hover:text-brand-600 transition">Inicio</a>  
                <a href="#productos" class="hover:text-brand-600 transition">Productos</a>  
                <a href="#beneficios" class="hover:text-brand-600 transition">¿Por qué Orgánico?</a>  
                <a href="#caja-custom" class="hover:text-brand-600 transition">Caja Mixta</a>  
                <a href="#contacto" class="hover:text-brand-600 transition">Contacto</a>  
            </nav>  
  
            <!-- Acciones de Carrito y Búsqueda -->  
            <div class="flex items-center gap-3">  
                <button onclick="toggleCartModal()" class="relative bg-brand-100 hover:bg-brand-200 text-brand-800 p-3 rounded-full transition flex items-center justify-center" aria-label="Ver Carrito">  
                    <i class="fa-solid fa-cart-shopping text-xl"></i>  
                    <span id="cart-count-badge" class="absolute -top-1 -right-1 bg-red-500 text-white text-xs w-5 h-5 rounded-full flex items-center justify-center font-bold shadow-sm">0</span>  
                </button>  
                <a href="#contacto" class="hidden sm:flex bg-brand-500 hover:bg-brand-600 text-white px-4 py-2.5 rounded-xl font-bold shadow-sm transition items-center gap-2">  
                    <i class="fa-solid fa-headset"></i> Pedir por Teléfono  
                </a>  
            </div>  
        </div>  
    </header>  
  
    <!-- Hero Section -->  
    <section id="inicio" class="relative bg-gradient-to-br from-brand-50 via-brand-bgWarm to-orange-100 py-12 md:py-20 overflow-hidden">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">  
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">  
                <div class="space-y-6 text-center lg:text-left">  
                    <div class="inline-flex items-center gap-2 bg-brand-green/10 text-brand-green px-4 py-1.5 rounded-full text-sm font-bold border border-brand-green/20">  
                        <i class="fa-solid fa-shield-cat"></i> 100% Orgánico, Sin Conservadores Ni Químicos  
                    </div>  
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-brand-800 leading-tight">  
                        Nutrición real y premios <span class="text-brand-500">deliciosos</span> para tu mejor amigo.  
                    </h1>  
                    <p class="text-lg text-gray-600 max-w-xl mx-auto lg:mx-0 font-medium">  
                        En <strong class="text-brand-700">PERRI SNACK</strong> horneamos diariamente botanas saludables con ingredientes de grado humano, carne magra, camote, avena y frutas frescas.  
                    </p>  
                    <div class="flex flex-col sm:flex-row gap-4 justify-center lg:justify-start">  
                        <a href="#productos" class="bg-brand-500 hover:bg-brand-600 text-white font-bold px-8 py-4 rounded-2xl shadow-lg hover:shadow-xl transition transform hover:-translate-y-0.5 text-center text-lg">  
                            <i class="fa-solid fa-bag-shopping mr-2"></i> Ver Menú de Snacks  
                        </a>  
                        <a href="tel:+528124129387" class="bg-white hover:bg-gray-50 text-brand-800 border-2 border-brand-500 font-bold px-6 py-4 rounded-2xl shadow-sm transition text-center text-lg flex items-center justify-center gap-2">  
                            <i class="fa-solid fa-phone text-brand-500"></i> Llama al 812-412-9387  
                        </a>  
                    </div>  
                    <!-- Badges -->  
                    <div class="pt-4 flex flex-wrap justify-center lg:justify-start gap-6 text-sm text-gray-700 font-semibold">  
                        <div class="flex items-center gap-2">  
                            <i class="fa-solid fa-check-circle text-brand-green text-lg"></i> Horneado Artesanal  
                        </div>  
                        <div class="flex items-center gap-2">  
                            <i class="fa-solid fa-check-circle text-brand-green text-lg"></i> Aprobado por Veterinarios  
                        </div>  
                        <div class="flex items-center gap-2">  
                            <i class="fa-solid fa-check-circle text-brand-green text-lg"></i> Hypoalergénico  
                        </div>  
                    </div>  
                </div>  
  
                <!-- Imagen Hero con overlay orgánico -->  
                <div class="relative flex justify-center">  
                    <div class="relative w-full max-w-md lg:max-w-none">  
                        <div class="absolute -top-6 -left-6 w-32 h-32 bg-yellow-300 rounded-full mix-blend-multiply filter blur-xl opacity-70 animate-pulse"></div>  
                        <div class="absolute -bottom-6 -right-6 w-32 h-32 bg-brand-green rounded-full mix-blend-multiply filter blur-xl opacity-30"></div>  
                        <img src="https://images.unsplash.com/photo-1583511655857-d19b40a7a54e?auto=format&fit=crop&w=1000&q=80"   
                             alt="Perrito feliz con snack orgánico"   
                             class="rounded-3xl shadow-2xl object-cover w-full h-[380px] sm:h-[450px] border-4 border-white"  
                             onerror="this.onerror=null; this.src='https://placehold.co/800x600/f3d8af/8f4618?text=PERRI+SNACK+Organic';">  
                          
                        <!-- Tarjeta flotante -->  
                        <div class="absolute bottom-4 left-4 bg-white/95 backdrop-blur-md p-4 rounded-2xl shadow-lg border border-orange-100 flex items-center gap-3 max-w-xs">  
                            <div class="w-12 h-12 bg-green-100 text-brand-green rounded-full flex items-center justify-center text-xl shrink-0">  
                                <i class="fa-solid fa-seedling"></i>  
                            </div>  
                            <div>  
                                <p class="text-xs text-gray-500 font-bold uppercase">Garantía de Frescura</p>  
                                <p class="text-sm font-bold text-gray-800">100% Carne Magra & Fruta Natural</p>  
                            </div>  
                        </div>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Sección Beneficios Orgánicos -->  
    <section id="beneficios" class="py-12 bg-white border-y border-gray-100">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <div class="text-center max-w-3xl mx-auto mb-10">  
                <h2 class="text-3xl font-extrabold text-brand-800">¿Por qué elegir los Snacks Orgánicos PERRI SNACK?</h2>  
                <p class="text-gray-600 mt-2">Cuidamos la digestión, el pelaje y la energía vital de tu mascota eliminando harina refinada, conservadores sintéticos y azúcares añadidos.</p>  
            </div>  
  
            <div class="grid grid-cols-1 md:grid-cols-4 gap-6">  
                <div class="bg-brand-50 p-6 rounded-2xl text-center border border-brand-100 hover:shadow-md transition">  
                    <div class="w-14 h-14 bg-brand-500 text-white rounded-2xl flex items-center justify-center text-2xl mx-auto mb-4">  
                        <i class="fa-solid fa-carrot"></i>  
                    </div>  
                    <h3 class="font-bold text-lg text-brand-800 mb-2">Ingredientes Reales</h3>  
                    <p class="text-sm text-gray-600">Camote, avena, manzana, arándanos, crema de cacahuate natural y proteínas de primera.</p>  
                </div>  
  
                <div class="bg-brand-50 p-6 rounded-2xl text-center border border-brand-100 hover:shadow-md transition">  
                    <div class="w-14 h-14 bg-brand-green text-white rounded-2xl flex items-center justify-center text-2xl mx-auto mb-4">  
                        <i class="fa-solid fa-stomach"></i>  
                    </div>  
                    <h3 class="font-bold text-lg text-brand-800 mb-2">Fácil Digestión</h3>  
                    <p class="text-sm text-gray-600">Ideal para mascotas con estómago sensible, alergias alimentarias o piel delicada.</p>  
                </div>  
  
                <div class="bg-brand-50 p-6 rounded-2xl text-center border border-brand-100 hover:shadow-md transition">  
                    <div class="w-14 h-14 bg-yellow-500 text-white rounded-2xl flex items-center justify-center text-2xl mx-auto mb-4">  
                        <i class="fa-solid fa-tooth"></i>  
                    </div>  
                    <h3 class="font-bold text-lg text-brand-800 mb-2">Salud Dental</h3>  
                    <p class="text-sm text-gray-600">Texturas crujientes que limpian el sarro de forma natural mientras disfrutan mordisquear.</p>  
                </div>  
  
                <div class="bg-brand-50 p-6 rounded-2xl text-center border border-brand-100 hover:shadow-md transition">  
                    <div class="w-14 h-14 bg-orange-600 text-white rounded-2xl flex items-center justify-center text-2xl mx-auto mb-4">  
                        <i class="fa-solid fa-heart-pulse"></i>  
                    </div>  
                    <h3 class="font-bold text-lg text-brand-800 mb-2">Cero Químicos</h3>  
                    <p class="text-sm text-gray-600">Sin colorantes, aromatizantes artificiales ni subproductos de origen industrial.</p>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Catálogo de Productos y Selección -->  
    <section id="productos" class="py-16 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-8 gap-4">  
            <div>  
                <span class="text-brand-green font-bold text-sm uppercase tracking-wider">Menú Fresco y Saludable</span>  
                <h2 class="text-3xl sm:text-4xl font-extrabold text-brand-800">Nuestros Snacks y Productos Orgánicos</h2>  
            </div>  
  
            <!-- Filtros de Categoría -->  
            <div class="flex flex-wrap gap-2" id="category-filters">  
                <button onclick="filterProducts('all')" class="filter-btn active bg-brand-500 text-white font-bold px-4 py-2 rounded-xl text-sm transition shadow-sm">Todos</button>  
                <button onclick="filterProducts('galletas')" class="filter-btn bg-white hover:bg-brand-100 text-gray-700 font-bold px-4 py-2 rounded-xl text-sm transition border border-gray-200">Galletas</button>  
                <button onclick="filterProducts('deshidratados')" class="filter-btn bg-white hover:bg-brand-100 text-gray-700 font-bold px-4 py-2 rounded-xl text-sm transition border border-gray-200">Deshidratados</button>  
                <button onclick="filterProducts('suplementos')" class="filter-btn bg-white hover:bg-brand-100 text-gray-700 font-bold px-4 py-2 rounded-xl text-sm transition border border-gray-200">Suplementos</button>  
                <button onclick="filterProducts('dentales')" class="filter-btn bg-white hover:bg-brand-100 text-gray-700 font-bold px-4 py-2 rounded-xl text-sm transition border border-gray-200">Dentales</button>  
            </div>  
        </div>  
  
        <!-- Rejilla de Productos Orgánicos -->  
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6" id="products-grid">  
            <!-- Los productos se inyectan dinámicamente mediante JS -->  
        </div>  
    </section>  
  
    <!-- Creador de Caja Mixta Personalizada -->  
    <section id="caja-custom" class="py-16 bg-gradient-to-r from-brand-800 to-brand-greenDark text-white my-8 rounded-3xl mx-4 sm:mx-8 px-6 sm:px-12 relative overflow-hidden shadow-2xl">  
        <div class="max-w-5xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-10 items-center relative z-10">  
            <div>  
                <span class="bg-yellow-400 text-brand-800 px-3 py-1 rounded-full text-xs font-bold uppercase tracking-wider">¡Nuevo Servicio Custom!</span>  
                <h2 class="text-3xl sm:text-4xl font-extrabold mt-3">Arma la Caja Orgánica Mixta de tu Mascota</h2>  
                <p class="text-orange-100 mt-3 text-sm sm:text-base">  
                    Selecciona el tamaño de tu peludo y sus ingredientes favoritos. Diseñamos una combinación fresca con empaque personalizado con su nombre.  
                </p>  
  
                <div class="mt-6 space-y-4 text-gray-800">  
                    <div>  
                        <label class="block text-white text-xs font-bold mb-1">Nombre de tu Mascota:</label>  
                        <input type="text" id="custom-pet-name" placeholder="Ej. Firulais / Maya" class="w-full px-4 py-2.5 rounded-xl text-sm focus:outline-none font-bold">  
                    </div>  
  
                    <div class="grid grid-cols-2 gap-3">  
                        <div>  
                            <label class="block text-white text-xs font-bold mb-1">Tamaño:</label>  
                            <select id="custom-size" onchange="calculateCustomBoxPrice()" class="w-full px-3 py-2.5 rounded-xl text-sm font-semibold bg-white">  
                                <option value="150">Chico (250g) - $150</option>  
                                <option value="260" selected>Mediano (500g) - $260</option>  
                                <option value="420">Grande (1kg) - $420</option>  
                            </select>  
                        </div>  
                        <div>  
                            <label class="block text-white text-xs font-bold mb-1">Proteína Principal:</label>  
                            <select id="custom-protein" class="w-full px-3 py-2.5 rounded-xl text-sm font-semibold bg-white">  
                                <option value="Pollo Orgánico">Pollo Orgánico</option>  
                                <option value="Res de Pastoreo">Res de Pastoreo</option>  
                                <option value="Salmón del Pacífico">Salmón Salvaje</option>  
                                <option value="Veggie (Camote y Avena)">Veggie Clean</option>  
                            </select>  
                        </div>  
                    </div>  
  
                    <div class="bg-white/10 p-4 rounded-2xl text-white backdrop-blur-sm border border-white/20">  
                        <div class="flex justify-between items-center font-bold">  
                            <span>Precio Total de la Caja:</span>  
                            <span id="custom-box-total" class="text-2xl text-yellow-300">$260.00 MXN</span>  
                        </div>  
                    </div>  
  
                    <button onclick="addCustomBoxToCart()" class="w-full bg-brand-500 hover:bg-brand-600 text-white font-extrabold py-3.5 rounded-xl shadow-lg transition flex items-center justify-center gap-2 text-base">  
                        <i class="fa-solid fa-box-open"></i> Agregar Caja Personalizada al Carrito  
                    </button>  
                </div>  
            </div>  
  
            <!-- Ilustración / Imagen de Caja -->  
            <div class="flex justify-center">  
                <div class="relative bg-white/10 p-6 rounded-3xl backdrop-blur-md border border-white/20 text-center w-full max-w-sm">  
                    <img src="https://images.unsplash.com/photo-1541599540903-216a46ca1dc0?auto=format&fit=crop&w=600&q=80"   
                         alt="Caja de snacks de perrito"   
                         class="rounded-2xl shadow-lg w-full h-56 object-cover mb-4"  
                         onerror="this.onerror=null; this.src='https://placehold.co/600x400/31572c/ffffff?text=PERRI+SNACK+BOX';">  
                    <div class="text-left bg-white p-3.5 rounded-xl text-gray-800">  
                        <p class="text-xs font-bold text-brand-green uppercase">Incluye gratis:</p>  
                        <p class="text-xs text-gray-600 mt-1">✓ Etiqueta con el nombre de tu mascota</p>  
                        <p class="text-xs text-gray-600">✓ Guía nutricional y de porciones</p>  
                        <p class="text-xs text-gray-600">✓ Regalo sorpresa saludable en tu primer pedido</p>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Sección de Contacto e Información de Compra Directa -->  
    <section id="contacto" class="py-16 bg-white border-t border-gray-100">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <div class="text-center max-w-2xl mx-auto mb-12">  
                <span class="bg-brand-100 text-brand-800 px-3 py-1 rounded-full text-xs font-bold uppercase">Atención Inmediata</span>  
                <h2 class="text-3xl font-extrabold text-brand-800 mt-2">¿Tienes dudas o deseas hacer un pedido especial?</h2>  
                <p class="text-gray-600 mt-2">Estamos listos para atenderte por teléfono, WhatsApp o formulario. Hacemos envíos locales e internacionales.</p>  
            </div>  
  
            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">  
                <!-- Tarjetas de Canales Rápidos -->  
                <div class="space-y-4">  
                    <!-- Teléfono Principal -->  
                    <a href="tel:+528124129387" class="block bg-brand-50 p-6 rounded-2xl border-2 border-brand-200 hover:border-brand-500 transition shadow-sm group">  
                        <div class="flex items-center gap-4">  
                            <div class="w-14 h-14 bg-brand-500 text-white rounded-2xl flex items-center justify-center text-2xl group-hover:scale-110 transition">  
                                <i class="fa-solid fa-phone-volume"></i>  
                            </div>  
                            <div>  
                                <h3 class="text-xs font-bold text-gray-500 uppercase">Llamada Directa</h3>  
                                <p class="text-xl font-extrabold text-brand-800">+52 (812) 412-9387</p>  
                                <span class="text-xs text-brand-green font-bold">Lun - Sáb: 8:00 AM - 8:00 PM</span>  
                            </div>  
                        </div>  
                    </a>  
  
                    <!-- WhatsApp -->  
                    <a href="https://wa.me/528124129387?text=Hola%20PERRI%20SNACK,%20quiero%20informacion%20sobre%20sus%20snacks%20organicos" target="_blank" class="block bg-green-50 p-6 rounded-2xl border-2 border-green-200 hover:border-green-500 transition shadow-sm group">  
                        <div class="flex items-center gap-4">  
                            <div class="w-14 h-14 bg-green-600 text-white rounded-2xl flex items-center justify-center text-2xl group-hover:scale-110 transition">  
                                <i class="fa-brands fa-whatsapp"></i>  
                            </div>  
                            <div>  
                                <h3 class="text-xs font-bold text-gray-500 uppercase">WhatsApp Ventas</h3>  
                                <p class="text-xl font-extrabold text-green-800">Enviar Mensaje</p>  
                                <span class="text-xs text-green-700 font-bold">Respuesta en menos de 5 minutos</span>  
                            </div>  
                        </div>  
                    </a>  
  
                    <!-- Dirección y Correo -->  
                    <div class="bg-gray-50 p-6 rounded-2xl border border-gray-200">  
                        <div class="space-y-3 text-sm">  
                            <div class="flex items-start gap-3">  
                                <i class="fa-solid fa-location-dot text-brand-500 text-lg mt-0.5"></i>  
                                <div>  
                                    <strong class="block text-gray-800">Oficina & Taller Orgánico:</strong>  
                                    <span class="text-gray-600">Calle 15 Av. 10 y 8 Col. Centro</span>  
                                </div>  
                            </div>  
                            <div class="flex items-center gap-3">  
                                <i class="fa-solid fa-envelope text-brand-500 text-lg"></i>  
                                <div>  
                                    <strong class="block text-gray-800">Correo Electrónico:</strong>  
                                    <span class="text-gray-600">contacto@perrisnack.com</span>  
                                </div>  
                            </div>  
                        </div>  
                    </div>  
                </div>  
  
                <!-- Formulario de Contacto -->  
                <div class="lg:col-span-2 bg-gray-50 p-6 sm:p-8 rounded-3xl border border-gray-200 shadow-sm">  
                    <h3 class="text-2xl font-bold text-brand-800 mb-4">Envíanos un mensaje rápido</h3>  
                    <form id="contact-form" onsubmit="handleContactSubmit(event)" class="space-y-4">  
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">  
                            <div>  
                                <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Nombre Completo *</label>  
                                <input type="text" required placeholder="Tu nombre" class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:outline-none focus:ring-2 focus:ring-brand-500 bg-white">  
                            </div>  
                            <div>  
                                <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Teléfono o WhatsApp *</label>  
                                <input type="tel" required placeholder="Ej. 271 000 0000" class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:outline-none focus:ring-2 focus:ring-brand-500 bg-white">  
                            </div>  
                        </div>  
  
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">  
                            <div>  
                                <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Nombre de tu Mascota</label>  
                                <input type="text" placeholder="Ej. Rocky / Lola" class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:outline-none focus:ring-2 focus:ring-brand-500 bg-white">  
                            </div>  
                            <div>  
                                <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Tipo de Mascota</label>  
                                <select class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:outline-none focus:ring-2 focus:ring-brand-500 bg-white">  
                                    <option value="perro">Perro</option>  
                                    <option value="gato">Gato</option>  
                                    <option value="ambos">Ambos / Varios</option>  
                                </select>  
                            </div>  
                        </div>  
  
                        <div>  
                            <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Mensaje o Pedido Especial *</label>  
                            <textarea required rows="3" placeholder="Escribe aquí tu consulta o los detalles de los productos que requieres..." class="w-full px-4 py-3 rounded-xl border border-gray-300 focus:outline-none focus:ring-2 focus:ring-brand-500 bg-white"></textarea>  
                        </div>  
  
                        <button type="submit" class="w-full bg-brand-green hover:bg-brand-greenDark text-white font-extrabold py-3.5 rounded-xl shadow-md transition flex items-center justify-center gap-2">  
                            <i class="fa-solid fa-paper-plane"></i> Enviar Mensaje  
                        </button>  
                    </form>  
                      
                    <div id="contact-success-msg" class="hidden mt-4 bg-green-100 border border-green-400 text-green-800 p-4 rounded-xl text-center font-bold">  
                        <i class="fa-solid fa-circle-check text-xl mr-2"></i> ¡Gracias por escribirnos! Un asesor de PERRI SNACK se comunicará contigo de inmediato.  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Testimonios de Clientes y Peluditos -->  
    <section class="py-12 bg-brand-50">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <h2 class="text-3xl font-extrabold text-brand-800 text-center mb-8">Lo que dicen los dueños enamorados de PERRI SNACK</h2>  
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">  
                  
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-brand-100">  
                    <div class="flex items-center gap-1 text-yellow-400 mb-3 text-sm">  
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>  
                    </div>  
                    <p class="text-gray-600 text-sm italic">"Mi perrita tiene alergia alimentaria severa a las galletas comerciales. Desde que probó las Galletas de Camote y Mantequilla de Maní de PERRI SNACK no ha vuelto a tener ronchas. ¡Excelente calidad!"</p>  
                    <div class="mt-4 flex items-center gap-3">  
                        <div class="w-10 h-10 bg-brand-200 rounded-full flex items-center justify-center font-bold text-brand-800">MC</div>  
                        <div>  
                            <h4 class="font-bold text-sm text-gray-800">María Fernanda C.</h4>  
                            <p class="text-xs text-gray-500">Mamá de "Max" (Beagle)</p>  
                        </div>  
                    </div>  
                </div>  
  
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-brand-100">  
                    <div class="flex items-center gap-1 text-yellow-400 mb-3 text-sm">  
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>  
                    </div>  
                    <p class="text-gray-600 text-sm italic">"Hice el pedido directo por teléfono y me llegó el mismo día a mi casa. El deshidratado de hígado orgánico es la obsesión de mi Golden. Recomendadísimos."</p>  
                    <div class="mt-4 flex items-center gap-3">  
                        <div class="w-10 h-10 bg-brand-200 rounded-full flex items-center justify-center font-bold text-brand-800">RG</div>  
                        <div>  
                            <h4 class="font-bold text-sm text-gray-800">Roberto Gómez</h4>  
                            <p class="text-xs text-gray-500">Papá de "Toby" (Golden Retriever)</p>  
                        </div>  
                    </div>  
                </div>  
  
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-brand-100">  
                    <div class="flex items-center gap-1 text-yellow-400 mb-3 text-sm">  
                        <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>  
                    </div>  
                    <p class="text-gray-600 text-sm italic">"Me encanta que sus ingredientes son de grado humano y transparentes. La caja personalizada con la etiqueta con el nombre de Maya fue un detalle hermoso."</p>  
                    <div class="mt-4 flex items-center gap-3">  
                        <div class="w-10 h-10 bg-brand-200 rounded-full flex items-center justify-center font-bold text-brand-800">AL</div>  
                        <div>  
                            <h4 class="font-bold text-sm text-gray-800">Andrea López</h4>  
                            <p class="text-xs text-gray-500">Mamá de "Maya" (Schnauzer)</p>  
                        </div>  
                    </div>  
                </div>  
  
            </div>  
        </div>  
    </section>  
  
    <!-- Pie de Página -->  
    <footer class="bg-brand-800 text-white mt-auto py-12">  
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">  
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 pb-8 border-b border-brand-700">  
                <div class="space-y-4">  
                    <div class="flex items-center gap-2">  
                        <div class="w-10 h-10 bg-brand-500 text-white rounded-xl flex items-center justify-center text-xl">  
                            <i class="fa-solid fa-bone"></i>  
                        </div>  
                        <span class="font-heading text-2xl font-bold tracking-wide">PERRI <span class="text-brand-500">SNACK</span></span>  
                    </div>  
                    <p class="text-sm text-orange-200">  
                        Pioneros en snacks orgánicos artesanales horneados con amor para la salud y felicidad de tus mejores amigos de cuatro patas.  
                    </p>  
                </div>  
  
                <div>  
                    <h4 class="font-bold text-lg mb-4 text-brand-500">Enlaces Rápidos</h4>  
                    <ul class="space-y-2 text-sm text-orange-100">  
                        <li><a href="#inicio" class="hover:text-white transition">Inicio</a></li>  
                        <li><a href="#productos" class="hover:text-white transition">Catálogo de Productos</a></li>  
                        <li><a href="#beneficios" class="hover:text-white transition">¿Por qué Orgánico?</a></li>  
                        <li><a href="#caja-custom" class="hover:text-white transition">Caja Mixta</a></li>  
                        <li><a href="#contacto" class="hover:text-white transition">Contacto</a></li>  
                    </ul>  
                </div>  
  
                <div>  
                    <h4 class="font-bold text-lg mb-4 text-brand-500">Atención Telefónica</h4>  
                    <p class="text-sm text-orange-100 mb-2">Haz tu pedido directo por llamada o WhatsApp:</p>  
                    <a href="tel:+528124129387" class="text-xl font-extrabold text-yellow-300 hover:underline block mb-2">  
                        <i class="fa-solid fa-phone mr-2"></i> +52 (812) 412-9387  
                    </a>  
                    <p class="text-xs text-orange-200">Lunes a Sábado de 8:00 AM a 8:00 PM</p>  
                </div>  
  
                <div>  
                    <h4 class="font-bold text-lg mb-4 text-brand-500">Síguenos en Redes</h4>  
                    <div class="flex gap-3 text-lg">  
                        <a href="#" class="w-10 h-10 bg-brand-700 hover:bg-brand-500 rounded-xl flex items-center justify-center transition" aria-label="Facebook"><i class="fa-brands fa-facebook-f"></i></a>  
                        <a href="#" class="w-10 h-10 bg-brand-700 hover:bg-brand-500 rounded-xl flex items-center justify-center transition" aria-label="Instagram"><i class="fa-brands fa-instagram"></i></a>  
                        <a href="#" class="w-10 h-10 bg-brand-700 hover:bg-brand-500 rounded-xl flex items-center justify-center transition" aria-label="TikTok"><i class="fa-brands fa-tiktok"></i></a>  
                        <a href="https://wa.me/528124129387" target="_blank" class="w-10 h-10 bg-green-600 hover:bg-green-500 rounded-xl flex items-center justify-center transition" aria-label="WhatsApp"><i class="fa-brands fa-whatsapp"></i></a>  
                    </div>  
                </div>  
            </div>  
  
            <div class="pt-6 text-center text-xs text-orange-300 flex flex-col sm:flex-row justify-between items-center gap-3">  
                <p>&copy; 2026 PERRI SNACK. Todos los derechos reservados. Productos 100% Orgánicos para Mascotas.</p>  
                <p>Hecho con amor para tus peluditos 🐶🐱</p>  
            </div>  
        </div>  
    </footer>  
  
    <!-- MODAL DE CARRITO DE COMPRAS (SIDE DRAWER) -->  
    <div id="cart-drawer" class="fixed inset-0 bg-black/60 z-50 opacity-0 pointer-events-none transition-opacity duration-300 flex justify-end">  
        <div id="cart-panel" class="bg-white w-full max-w-md h-full shadow-2xl flex flex-col transform translate-x-full transition-transform duration-300">  
            <!-- Header Carrito -->  
            <div class="p-4 sm:p-6 bg-brand-800 text-white flex justify-between items-center">  
                <div class="flex items-center gap-2">  
                    <i class="fa-solid fa-cart-shopping text-xl text-brand-500"></i>  
                    <h3 class="text-xl font-bold">Tu Carrito PERRI SNACK</h3>  
                </div>  
                <button onclick="toggleCartModal()" class="text-gray-300 hover:text-white text-2xl font-bold" aria-label="Cerrar">&times;</button>  
            </div>  
  
            <!-- Lista de items agregados -->  
            <div id="cart-items-container" class="flex-1 p-4 overflow-y-auto custom-scrollbar space-y-4">  
                <!-- Inyectado dinámicamente -->  
            </div>  
  
            <!-- Footer Carrito con Subtotal y Botón Comprar -->  
            <div class="p-6 bg-gray-50 border-t border-gray-200 space-y-4">  
                <div class="space-y-2 text-sm">  
                    <div class="flex justify-between text-gray-600">  
                        <span>Subtotal:</span>  
                        <span id="cart-subtotal font-bold">$0.00</span>  
                    </div>  
                    <div class="flex justify-between text-gray-600">  
                        <span>Envío estimado:</span>  
                        <span id="cart-shipping" class="text-brand-green font-bold">Gratis</span>  
                    </div>  
                    <div class="flex justify-between text-lg font-extrabold text-brand-800 pt-2 border-t border-gray-200">  
                        <span>Total a pagar:</span>  
                        <span id="cart-total">$0.00 MXN</span>  
                    </div>  
                </div>  
  
                <button id="checkout-btn" onclick="openCheckoutModal()" class="w-full bg-brand-500 hover:bg-brand-600 text-white font-extrabold py-3.5 rounded-xl shadow-lg transition flex items-center justify-center gap-2 text-base">  
                    <i class="fa-solid fa-credit-card"></i> Proceder al Pago / Comprar  
                </button>  
                <button onclick="toggleCartModal()" class="w-full text-center text-xs text-gray-500 hover:underline">  
                    Seguir viendo más snacks  
                </button>  
            </div>  
        </div>  
    </div>  
  
    <!-- MODAL DE CHECKOUT / FINALIZAR COMPRA -->  
    <div id="checkout-modal" class="fixed inset-0 bg-black/70 z-50 flex items-center justify-center p-4 hidden">  
        <div class="bg-white rounded-3xl max-w-lg w-full p-6 sm:p-8 shadow-2xl relative max-h-[90vh] overflow-y-auto custom-scrollbar">  
            <button onclick="closeCheckoutModal()" class="absolute top-4 right-4 text-gray-400 hover:text-gray-700 text-2xl font-bold">&times;</button>  
  
            <div class="text-center mb-6">  
                <div class="w-12 h-12 bg-brand-100 text-brand-500 rounded-full flex items-center justify-center text-2xl mx-auto mb-2">  
                    <i class="fa-solid fa-bag-shopping"></i>  
                </div>  
                <h3 class="text-2xl font-extrabold text-brand-800">Finalizar Pedido PERRI SNACK</h3>  
                <p class="text-xs text-gray-500">Completa tus datos para enviarte tus productos orgánicos</p>  
            </div>  
  
            <form id="checkout-form" onsubmit="processOrder(event)" class="space-y-4">  
                <div>  
                    <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Nombre Completo *</label>  
                    <input type="text" required placeholder="Juan Pérez" class="w-full px-4 py-2.5 border border-gray-300 rounded-xl text-sm focus:ring-2 focus:ring-brand-500 outline-none">  
                </div>  
  
                <div class="grid grid-cols-2 gap-3">  
                    <div>  
                        <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Teléfono / WhatsApp *</label>  
                        <input type="tel" required placeholder="271 123 4567" class="w-full px-4 py-2.5 border border-gray-300 rounded-xl text-sm focus:ring-2 focus:ring-brand-500 outline-none">  
                    </div>  
                    <div>  
                        <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Ciudad / Municipio *</label>  
                        <input type="text" required placeholder="Córdoba, Ver." class="w-full px-4 py-2.5 border border-gray-300 rounded-xl text-sm focus:ring-2 focus:ring-brand-500 outline-none">  
                    </div>  
                </div>  
  
                <div>  
                    <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Dirección Completa de Entrega *</label>  
                    <input type="text" required placeholder="Calle, número exterior/interior, colonia y C.P." class="w-full px-4 py-2.5 border border-gray-300 rounded-xl text-sm focus:ring-2 focus:ring-brand-500 outline-none">  
                </div>  
  
                <div>  
                    <label class="block text-xs font-bold text-gray-700 uppercase mb-1">Método de Pago Preferido</label>  
                    <select id="payment-method" class="w-full px-4 py-2.5 border border-gray-300 rounded-xl text-sm font-semibold focus:ring-2 focus:ring-brand-500 outline-none bg-white">  
                        <option value="efectivo">Pago contra entrega / Efectivo</option>  
                        <option value="transferencia">Transferencia SPEI / Banco</option>  
                        <option value="tarjeta">Tarjeta Débito/Crédito al entregar</option>  
                    </select>  
                </div>  
  
                <div class="bg-brand-50 p-4 rounded-2xl border border-brand-200">  
                    <div class="flex justify-between items-center font-bold text-brand-800 text-sm">  
                        <span>Resumen a Pagar:</span>  
                        <span id="checkout-final-total" class="text-xl text-brand-500">$0.00 MXN</span>  
                    </div>  
                </div>  
  
                <button type="submit" class="w-full bg-brand-green hover:bg-brand-greenDark text-white font-extrabold py-3.5 rounded-xl shadow-lg transition text-center text-base">  
                    <i class="fa-solid fa-check-circle mr-1"></i> Confirmar y Realizar Pedido  
                </button>  
            </form>  
  
            <div id="order-success-screen" class="hidden text-center py-6 space-y-4">  
                <div class="w-16 h-16 bg-green-100 text-green-600 rounded-full flex items-center justify-center text-3xl mx-auto">  
                    <i class="fa-solid fa-circle-check"></i>  
                </div>  
                <h3 class="text-2xl font-extrabold text-brand-800">¡Pedido Recibido con Éxito!</h3>  
                <p class="text-sm text-gray-600">  
                    Hemos registrado tu compra. En breve nos comunicaremos a tu teléfono para confirmar el envío fresco de tus snacks.  
                </p>  
                <div class="bg-gray-100 p-3 rounded-xl text-xs font-mono text-gray-700">  
                    FOLIO DE PEDIDO: <span id="order-folio" class="font-bold text-brand-800">#PS-8921</span>  
                </div>  
                <button onclick="closeCheckoutModal(); resetCart();" class="w-full bg-brand-500 text-white font-bold py-3 rounded-xl">  
                    Volver a la Tienda  
                </button>  
            </div>  
        </div>  
    </div>  
  
    <!-- TOAST NOTIFICATION -->  
    <div id="toast" class="fixed bottom-5 right-5 bg-brand-800 text-white px-5 py-3.5 rounded-2xl shadow-2xl z-50 flex items-center gap-3 transform translate-y-20 opacity-0 transition-all duration-300 border border-brand-500">  
        <i class="fa-solid fa-paw text-yellow-400 text-xl"></i>  
        <div>  
            <p id="toast-message" class="text-sm font-bold">¡Producto agregado al carrito!</p>  
        </div>  
    </div>  
  
    <script>  
        // BASE DE DATOS DE PRODUCTOS ORGANICOS PERRI SNACK  
        const products = [  
            {  
                id: 1,  
                name: "Galletas de Camote y Mantequilla de Maní",  
                category: "galletas",  
                price: 110,  
                rating: 5.0,  
                weight: "200g",  
                organicBadge: "100% Orgánico",  
                image: "https://images.unsplash.com/photo-1568640347023-a616a30bc3bd?auto=format&fit=crop&w=600&q=80",  
                description: "Horneadas a fuego lento. Ricas en fibra y grasas saludables para pelaje brillante."  
            },  
            {  
                id: 2,  
                name: "Snacks Deshidratados de Hígado de Pollo",  
                category: "deshidratados",  
                price: 145,  
                rating: 4.9,  
                weight: "150g",  
                organicBadge: "Proteína Purísima",  
                image: "https://images.unsplash.com/photo-1582562124811-c09040d0a901?auto=format&fit=crop&w=600&q=80",  
                description: "100% pechuga e hígado de pollo orgánico deshidratado. Ideal para entrenamiento."  
            },  
            {  
                id: 3,  
                name: "Bites Orgánicos de Salmón y Espinaca",  
                category: "deshidratados",  
                price: 165,  
                rating: 4.8,  
                weight: "180g",  
                organicBadge: "Rico en Omega-3",  
                image: "https://images.unsplash.com/photo-1548767797-d8c844163c4c?auto=format&fit=crop&w=600&q=80",  
                description: "Favorito de perros y gatos. Promueve articulaciones fuertes y salud cardiovascular."  
            },  
            {  
                id: 4,  
                name: "Premios Dentales de Manzana y Canela",  
                category: "dentales",  
                price: 95,  
                rating: 4.9,  
                weight: "220g",  
                organicBadge: "Aliento Fresco",  
                image: "https://images.unsplash.com/photo-1535294435445-d7249524ef2e?auto=format&fit=crop&w=600&q=80",  
                description: "Combate el sarro de manera mecánica e higieniza el aliento de forma natural."  
            },  
            {  
                id: 5,  
                name: "Aceite Orgánico de Salmón Salvaje",  
                category: "suplementos",  
                price: 280,  
                rating: 5.0,  
                weight: "250ml",  
                organicBadge: "Suplemento Premium",  
                image: "https://images.unsplash.com/photo-1608248597309-a1b7e937d578?auto=format&fit=crop&w=600&q=80",  
                description: "Sazonador natural para sus croquetas o alimento BARF. Cero aditivos químicos."  
            },  
            {  
                id: 6,  
                name: "Chew Sticks Orgánicos de Calabaza y Avena",  
                category: "dentales",  
                price: 120,  
                rating: 4.7,  
                weight: "200g",  
                organicBadge: "Salud Digestiva",  
                image: "https://images.unsplash.com/photo-1583511655826-05700d52f4d9?auto=format&fit=crop&w=600&q=80",  
                description: "Barritas masticables crujientes para calmar la ansiedad y favorecer la digestión."  
            },  
            {  
                id: 7,  
                name: "Snacks Deshidratados de Pulmón de Res",  
                category: "deshidratados",  
                price: 135,  
                rating: 4.9,  
                weight: "120g",  
                organicBadge: "Bajo en Grasa",  
                image: "https://images.unsplash.com/photo-1583337130417-3346a1be7dee?auto=format&fit=crop&w=600&q=80",  
                description: "Premios ligeros y crujientes ideales para perros de edad avanzada o con dieta estricta."  
            },  
            {  
                id: 8,  
                name: "Galletas de Zanahoria, Cúrcuma y Coco",  
                category: "galletas",  
                price: 105,  
                rating: 4.8,  
                weight: "200g",  
                organicBadge: "Antiinflamatorio",  
                image: "https://images.unsplash.com/photo-1543466835-00a7907e9de1?auto=format&fit=crop&w=600&q=80",  
                description: "Súper alimentos combinados para proteger articulaciones e inmunidad."  
            }  
        ];  
  
        // ESTADO DEL CARRITO  
        let cart = [];  
  
        // RENDERIZAR PRODUCTOS  
        function renderProducts(filter = 'all') {  
            const grid = document.getElementById('products-grid');  
            grid.innerHTML = '';  
  
            const filtered = filter === 'all'   
                ? products   
                : products.filter(p => p.category === filter);  
  
            filtered.forEach(p => {  
                const card = document.createElement('div');  
                card.className = "bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition duration-300 border border-gray-100 flex flex-col justify-between group";  
                card.innerHTML = `  
                    <div>  
                        <!-- Imagen y badges -->  
                        <div class="relative overflow-hidden h-48 bg-gray-100">  
                            <img src="${p.image}" alt="${p.name}" class="w-full h-full object-cover group-hover:scale-105 transition duration-500" onerror="this.onerror=null; this.src='https://placehold.co/600x400/f9edd8/b55e17?text=PERRI+SNACK';">  
                            <span class="absolute top-3 left-3 bg-brand-green text-white text-[10px] font-extrabold px-2.5 py-1 rounded-full shadow-sm uppercase tracking-wider">  
                                ${p.organicBadge}  
                            </span>  
                            <span class="absolute top-3 right-3 bg-white/90 backdrop-blur-md text-gray-700 text-xs font-bold px-2 py-0.5 rounded-lg shadow-sm">  
                                <i class="fa-solid fa-weight-hanging text-brand-500 mr-1"></i>${p.weight}  
                            </span>  
                        </div>  
  
                        <!-- Info del Producto -->  
                        <div class="p-5">  
                            <div class="flex items-center justify-between mb-1">  
                                <span class="text-xs text-brand-600 font-bold uppercase tracking-wider">${p.category}</span>  
                                <div class="flex items-center gap-1 text-xs text-yellow-500 font-bold">  
                                    <i class="fa-solid fa-star"></i> ${p.rating}  
                                </div>  
                            </div>  
  
                            <h3 class="font-extrabold text-gray-800 text-lg leading-snug group-hover:text-brand-600 transition mb-2">  
                                ${p.name}  
                            </h3>  
  
                            <p class="text-xs text-gray-500 line-clamp-2 mb-4">  
                                ${p.description}  
                            </p>  
                        </div>  
                    </div>  
  
                    <!-- Precio y Selección de Compra -->  
                    <div class="p-5 pt-0 border-t border-gray-50 flex items-center justify-between mt-auto">  
                        <div>  
                            <span class="text-xs text-gray-400 block font-bold">Precio Unitario</span>  
                            <span class="text-2xl font-extrabold text-brand-800">$${p.price}.00 <span class="text-xs text-gray-500 font-normal">MXN</span></span>  
                        </div>  
                        <button onclick="addToCart(${p.id})" class="bg-brand-500 hover:bg-brand-600 text-white font-bold p-3 rounded-2xl shadow-md transition transform hover:scale-105 flex items-center justify-center" title="Agregar al Carrito">  
                            <i class="fa-solid fa-cart-plus text-lg"></i>  
                        </button>  
                    </div>  
                `;  
                grid.appendChild(card);  
            });  
        }  
  
        // FILTRADO  
        function filterProducts(category) {  
            document.querySelectorAll('.filter-btn').forEach(btn => {  
                btn.classList.remove('bg-brand-500', 'text-white');  
                btn.classList.add('bg-white', 'text-gray-700');  
            });  
  
            event.target.classList.remove('bg-white', 'text-gray-700');  
            event.target.classList.add('bg-brand-500', 'text-white');  
  
            renderProducts(category);  
        }  
  
        // FUNCIONES DE CARRITO  
        function addToCart(productId) {  
            const product = products.find(p => p.id === productId);  
            const existingIndex = cart.findIndex(item => item.id === productId);  
  
            if (existingIndex > -1) {  
                cart[existingIndex].quantity += 1;  
            } else {  
                cart.push({ ...product, quantity: 1 });  
            }  
  
            updateCartUI();  
            showToast(`¡"${product.name}" agregado al carrito!`);  
        }  
  
        function updateQuantity(productId, delta) {  
            const index = cart.findIndex(item => item.id === productId);  
            if (index > -1) {  
                cart[index].quantity += delta;  
                if (cart[index].quantity <= 0) {  
                    cart.splice(index, 1);  
                }  
            }  
            updateCartUI();  
        }  
  
        function removeFromCart(productId) {  
            cart = cart.filter(item => item.id !== productId);  
            updateCartUI();  
            showToast("Producto eliminado del carrito");  
        }  
  
        function updateCartUI() {  
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);  
            document.getElementById('cart-count-badge').innerText = totalItems;  
  
            const container = document.getElementById('cart-items-container');  
            container.innerHTML = '';  
  
            if (cart.length === 0) {  
                container.innerHTML = `  
                    <div class="text-center py-12 text-gray-400">  
                        <i class="fa-solid fa-basket-shopping text-5xl mb-3 text-brand-200"></i>  
                        <p class="font-bold text-gray-600">Tu carrito está vacío</p>  
                        <p class="text-xs mt-1">¡Añade premios orgánicos para tu peludito!</p>  
                    </div>  
                `;  
            } else {  
                cart.forEach(item => {  
                    const itemEl = document.createElement('div');  
                    itemEl.className = "flex items-center gap-3 bg-gray-50 p-3 rounded-2xl border border-gray-200";  
                    itemEl.innerHTML = `  
                        <img src="${item.image}" alt="${item.name}" class="w-16 h-16 rounded-xl object-cover shrink-0">  
                        <div class="flex-1">  
                            <h4 class="font-bold text-sm text-gray-800 line-clamp-1">${item.name}</h4>  
                            <p class="text-xs text-brand-600 font-extrabold">$${item.price}.00 c/u</p>  
                            <div class="flex items-center gap-2 mt-1">  
                                <button onclick="updateQuantity(${item.id}, -1)" class="w-6 h-6 bg-gray-200 hover:bg-gray-300 rounded-lg text-xs font-bold">-</button>  
                                <span class="text-xs font-bold w-4 text-center">${item.quantity}</span>  
                                <button onclick="updateQuantity(${item.id}, 1)" class="w-6 h-6 bg-brand-200 hover:bg-brand-300 rounded-lg text-xs font-bold text-brand-800">+</button>  
                            </div>  
                        </div>  
                        <div class="text-right">  
                            <p class="font-extrabold text-sm text-gray-800">$${item.price * item.quantity}.00</p>  
                            <button onclick="removeFromCart(${item.id})" class="text-red-400 hover:text-red-600 text-xs mt-1">  
                                <i class="fa-solid fa-trash-can"></i>  
                            </button>  
                        </div>  
                    `;  
                    container.appendChild(itemEl);  
                });  
            }  
  
            const subtotal = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);  
            document.getElementById('cart-subtotal').innerText = `$${subtotal}.00 MXN`;  
            document.getElementById('cart-total').innerText = `$${subtotal}.00 MXN`;  
            document.getElementById('checkout-final-total').innerText = `$${subtotal}.00 MXN`;  
        }  
  
        // CAJA CUSTOMIZADA  
        function calculateCustomBoxPrice() {  
            const price = document.getElementById('custom-size').value;  
            document.getElementById('custom-box-total').innerText = `$${price}.00 MXN`;  
        }  
  
        function addCustomBoxToCart() {  
            const petName = document.getElementById('custom-pet-name').value || "Mascota";  
            const price = parseInt(document.getElementById('custom-size').value);  
            const protein = document.getElementById('custom-protein').value;  
  
            const customItem = {  
                id: Date.now(),  
                name: `Caja Mixta Orgánica (${petName}) - ${protein}`,  
                price: price,  
                quantity: 1,  
                image: "https://images.unsplash.com/photo-1541599540903-216a46ca1dc0?auto=format&fit=crop&w=600&q=80"  
            };  
  
            cart.push(customItem);  
            updateCartUI();  
            toggleCartModal();  
            showToast(`¡Caja Mixta para ${petName} agregada!`);  
        }  
  
        // INTERFAZ MODALES  
        function toggleCartModal() {  
            const drawer = document.getElementById('cart-drawer');  
            const panel = document.getElementById('cart-panel');  
  
            if (drawer.classList.contains('pointer-events-none')) {  
                drawer.classList.remove('pointer-events-none', 'opacity-0');  
                drawer.classList.add('opacity-100');  
                panel.classList.remove('translate-x-full');  
            } else {  
                drawer.classList.add('pointer-events-none', 'opacity-0');  
                drawer.classList.remove('opacity-100');  
                panel.classList.add('translate-x-full');  
            }  
        }  
  
        function openCheckoutModal() {  
            if (cart.length === 0) {  
                showToast("Primero agrega al menos un snack al carrito");  
                return;  
            }  
            toggleCartModal();  
            document.getElementById('checkout-modal').classList.remove('hidden');  
        }  
  
        function closeCheckoutModal() {  
            document.getElementById('checkout-modal').classList.add('hidden');  
            document.getElementById('checkout-form').classList.remove('hidden');  
            document.getElementById('order-success-screen').classList.add('hidden');  
        }  
  
        function processOrder(e) {  
            e.preventDefault();  
            const folio = "#PS-" + Math.floor(1000 + Math.random() * 9000);  
            document.getElementById('order-folio').innerText = folio;  
            document.getElementById('checkout-form').classList.add('hidden');  
            document.getElementById('order-success-screen').classList.remove('hidden');  
        }  
  
        function resetCart() {  
            cart = [];  
            updateCartUI();  
        }  
  
        function handleContactSubmit(e) {  
            e.preventDefault();  
            const msg = document.getElementById('contact-success-msg');  
            msg.classList.remove('hidden');  
            e.target.reset();  
            setTimeout(() => {  
                msg.classList.add('hidden');  
            }, 6000);  
        }  
  
        function showToast(message) {  
            const toast = document.getElementById('toast');  
            document.getElementById('toast-message').innerText = message;  
            toast.classList.remove('translate-y-20', 'opacity-0');  
            toast.classList.add('translate-y-0', 'opacity-100');  
  
            setTimeout(() => {  
                toast.classList.add('translate-y-20', 'opacity-0');  
                toast.classList.remove('translate-y-0', 'opacity-100');  
            }, 3000);  
        }  
  
        // INICIALIZACIÓN  
        window.onload = function() {  
            renderProducts();  
            updateCartUI();  
        };  
    </script>  
</body>  
</html>  
