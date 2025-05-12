<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dunun Percusión - Instrumentos de Percusión Brasileña</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Montserrat', sans-serif;
            scroll-behavior: smooth;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #FF5F6D 0%, #FFC371 100%);
        }
        
        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .dropdown:hover .dropdown-menu {
            display: block;
        }
        
        .carousel-item {
            transition: opacity 0.5s ease;
        }
        
        .carousel-item:not(.active) {
            opacity: 0;
            display: none;
        }
        
        .instagram-feed {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 10px;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Header -->
    <header class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <a href="#" class="flex items-center">
                    <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxwpPA7SiewfwKZ8ILQdR_Pl03O6USBv2TaB6yWr5ImOU5Hw18umHhYvB6aulxNv7Lwds&usqp=CAU" alt="Dunun Percusión Logo" class="h-10 mr-2">

                    <span class="text-xl font-bold text-orange-600">Dunun Percusión</span>
                </a>
            </div>
            
            <div class="hidden md:flex space-x-6">
                <div class="dropdown relative">
                    <button class="text-gray-700 hover:text-orange-600 font-medium flex items-center">
                        Productos <i class="fas fa-chevron-down ml-1 text-xs"></i>
                    </button>
                    <div class="dropdown-menu absolute hidden bg-white shadow-lg rounded-md mt-2 py-2 w-48">
                        <a href="#" class="block px-4 py-2 text-gray-700 hover:bg-orange-50 hover:text-orange-600">Surdos</a>
                        <a href="#" class="block px-4 py-2 text-gray-700 hover:bg-orange-50 hover:text-orange-600">Repiniques</a>
                        <a href="#" class="block px-4 py-2 text-gray-700 hover:bg-orange-50 hover:text-orange-600">Caixas</a>
                        <a href="#" class="block px-4 py-2 text-gray-700 hover:bg-orange-50 hover:text-orange-600">Tamborins</a>
                        <a href="#" class="block px-4 py-2 text-gray-700 hover:bg-orange-50 hover:text-orange-600">Accesorios</a>
                    </div>
                </div>
                <a href="#" class="text-gray-700 hover:text-orange-600 font-medium">Sobre Nosotros</a>
                <a href="#" class="text-gray-700 hover:text-orange-600 font-medium">Talleres</a>
                <a href="#" class="text-gray-700 hover:text-orange-600 font-medium">Contacto</a>
            </div>
            
            <div class="flex items-center space-x-4">
                <a href="#" class="text-gray-700 hover:text-orange-600">
                    <i class="fas fa-search"></i>
                </a>
                <a href="#" class="text-gray-700 hover:text-orange-600 relative">
                    <i class="fas fa-shopping-cart"></i>
                    <span class="absolute -top-2 -right-2 bg-orange-500 text-white text-xs rounded-full h-5 w-5 flex items-center justify-center">3</span>
                </a>
                <button class="md:hidden text-gray-700" id="mobile-menu-button">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
        </div>
        
        <!-- Mobile menu -->
        <div class="md:hidden hidden bg-white shadow-lg" id="mobile-menu">
            <div class="px-4 py-3 space-y-3">
                <div class="dropdown">
                    <button class="w-full text-left text-gray-700 font-medium flex justify-between items-center">
                        Productos <i class="fas fa-chevron-down ml-1 text-xs"></i>
                    </button>
                    <div class="dropdown-menu hidden pl-4 mt-2 space-y-2">
                        <a href="#" class="block text-gray-700 hover:text-orange-600">Surdos</a>
                        <a href="#" class="block text-gray-700 hover:text-orange-600">Repiniques</a>
                        <a href="#" class="block text-gray-700 hover:text-orange-600">Caixas</a>
                        <a href="#" class="block text-gray-700 hover:text-orange-600">Tamborins</a>
                        <a href="#" class="block text-gray-700 hover:text-orange-600">Accesorios</a>
                    </div>
                </div>
                <a href="#" class="block text-gray-700 hover:text-orange-600">Sobre Nosotros</a>
                <a href="#" class="block text-gray-700 hover:text-orange-600">Talleres</a>
                <a href="#" class="block text-gray-700 hover:text-orange-600">Contacto</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-gradient text-white py-16 md:py-24">
        <div class="container mx-auto px-4 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-8 md:mb-0">
                <h1 class="text-4xl md:text-5xl font-bold mb-4">Instrumentos de Percusión Brasileña</h1>
                <p class="text-xl mb-6">Descubre la auténtica esencia del batucada con nuestros instrumentos artesanales de alta calidad.</p>
                <div class="flex space-x-4">
                    <a href="#productos" class="bg-white text-orange-600 px-6 py-3 rounded-full font-medium hover:bg-gray-100 transition">Ver Productos</a>
                    <a href="#contacto" class="border-2 border-white px-6 py-3 rounded-full font-medium hover:bg-white hover:bg-opacity-20 transition">Contactar</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSusjgIHQJXe72ZyFzVN7X12T4-_fjFo0yZSw&s" alt="Batucada Group" class="rounded-lg shadow-xl max-w-full h-auto">
            </div>
        </div>
    </section>

    <!-- Featured Categories -->
    <section class="py-12 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Nuestras Categorías</h2>
            <div class="grid grid-cols-2 md:grid-cols-5 gap-6">
                <a href="#" class="bg-gray-50 rounded-lg p-4 text-center hover:shadow-md transition">
                    <div class="bg-orange-100 rounded-full h-16 w-16 mx-auto mb-3 flex items-center justify-center">
                        <i class="fas fa-drum text-orange-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium">Surdos</h3>
                </a>
                <a href="#" class="bg-gray-50 rounded-lg p-4 text-center hover:shadow-md transition">
                    <div class="bg-orange-100 rounded-full h-16 w-16 mx-auto mb-3 flex items-center justify-center">
                        <i class="fas fa-drum text-orange-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium">Repiniques</h3>
                </a>
                <a href="#" class="bg-gray-50 rounded-lg p-4 text-center hover:shadow-md transition">
                    <div class="bg-orange-100 rounded-full h-16 w-16 mx-auto mb-3 flex items-center justify-center">
                        <i class="fas fa-drum text-orange-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium">Caixas</h3>
                </a>
                <a href="#" class="bg-gray-50 rounded-lg p-4 text-center hover:shadow-md transition">
                    <div class="bg-orange-100 rounded-full h-16 w-16 mx-auto mb-3 flex items-center justify-center">
                        <i class="fas fa-drum text-orange-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium">Tamborins</h3>
                </a>
                <a href="#" class="bg-gray-50 rounded-lg p-4 text-center hover:shadow-md transition">
                    <div class="bg-orange-100 rounded-full h-16 w-16 mx-auto mb-3 flex items-center justify-center">
                        <i class="fas fa-drum text-orange-600 text-2xl"></i>
                    </div>
                    <h3 class="font-medium">Accesorios</h3>
                </a>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section id="productos" class="py-12 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="flex justify-between items-center mb-8">
                <h2 class="text-3xl font-bold">Nuestros Productos</h2>
                <div class="flex space-x-2">
                    <button class="px-4 py-2 bg-white rounded-md border hover:bg-gray-100">Todos</button>
                    <button class="px-4 py-2 bg-white rounded-md border hover:bg-gray-100">Popular</button>
                    <button class="px-4 py-2 bg-white rounded-md border hover:bg-gray-100">Nuevo</button>
                </div>
            </div>
            
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8">
                <!-- Product 1 -->
                <div class="product-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="relative">
                        <img src="blob:https://web.whatsapp.com/1fd6ad24-3e50-4ee5-b872-646350ebd863" alt="Surdo 22''" class="w-full h-64 object-cover">

                        <div class="absolute top-2 right-2 bg-orange-500 text-white text-xs px-2 py-1 rounded-full">Nuevo</div>
                    </div>
                    <div class="p-4">
                        <div class="flex justify-between items-start">
                            <div>
                                <h3 class="font-bold text-lg">Surdo 22''</h3>
                                <p class="text-gray-600 text-sm">Percusión brasileña</p>
                            </div>
                            <div class="text-orange-600 font-bold">$350.000</div>
                        </div>
                        <div class="mt-4 flex justify-between items-center">
                            <button class="bg-orange-500 text-white px-4 py-2 rounded-full text-sm hover:bg-orange-600 transition">Añadir al carrito</button>
                            <button class="text-gray-400 hover:text-orange-500">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                    </div>
                </div>
                
                <!-- Product 2 -->
                <div class="product-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="relative">
                        <img src="https://via.placeholder.com/300x300" alt="Repinique 12''" class="w-full h-64 object-cover">
                        <div class="absolute top-2 right-2 bg-orange-500 text-white text-xs px-2 py-1 rounded-full">Popular</div>
                    </div>
                    <div class="p-4">
                        <div class="flex justify-between items-start">
                            <div>
                                <h3 class="font-bold text-lg">Repinique 12''</h3>
                                <p class="text-gray-600 text-sm">Percusión brasileña</p>
                            </div>
                            <div class="text-orange-600 font-bold">$280.000</div>
                        </div>
                        <div class="mt-4 flex justify-between items-center">
                            <button class="bg-orange-500 text-white px-4 py-2 rounded-full text-sm hover:bg-orange-600 transition">Añadir al carrito</button>
                            <button class="text-gray-400 hover:text-orange-500">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                    </div>
                </div>
                
                <!-- Product 3 -->
                <div class="product-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="relative">
                        <img src="https://via.placeholder.com/300x300" alt="Caixa 14''" class="w-full h-64 object-cover">
                    </div>
                    <div class="p-4">
                        <div class="flex justify-between items-start">
                            <div>
                                <h3 class="font-bold text-lg">Caixa 14''</h3>
                                <p class="text-gray-600 text-sm">Percusión brasileña</p>
                            </div>
                            <div class="text-orange-600 font-bold">$320.000</div>
                        </div>
                        <div class="mt-4 flex justify-between items-center">
                            <button class="bg-orange-500 text-white px-4 py-2 rounded-full text-sm hover:bg-orange-600 transition">Añadir al carrito</button>
                            <button class="text-gray-400 hover:text-orange-500">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                    </div>
                </div>
                
                <!-- Product 4 -->
                <div class="product-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="relative">
                        <img src="https://via.placeholder.com/300x300" alt="Tamborim" class="w-full h-64 object-cover">
                    </div>
                    <div class="p-4">
                        <div class="flex justify-between items-start">
                            <div>
                                <h3 class="font-bold text-lg">Tamborim</h3>
                                <p class="text-gray-600 text-sm">Percusión brasileña</p>
                            </div>
                            <div class="text-orange-600 font-bold">$120.000</div>
                        </div>
                        <div class="mt-4 flex justify-between items-center">
                            <button class="bg-orange-500 text-white px-4 py-2 rounded-full text-sm hover:bg-orange-600 transition">Añadir al carrito</button>
                            <button class="text-gray-400 hover:text-orange-500">
                                <i class="far fa-heart"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="text-center mt-10">
                <a href="#" class="inline-block border-2 border-orange-500 text-orange-500 px-6 py-3 rounded-full font-medium hover:bg-orange-500 hover:text-white transition">Ver todos los productos</a>
            </div>
        </div>
    </section>

    <!-- Product Detail Example (would be a separate page in reality) -->
    <section class="py-12 bg-white hidden" id="product-detail">
        <div class="container mx-auto px-4">
            <div class="grid md:grid-cols-2 gap-12">
                <div>
                    <!-- Product Carousel -->
                    <div class="carousel relative">
                        <div class="carousel-item active">
                            <img src="https://via.placeholder.com/600x600" alt="Surdo 22''" class="w-full rounded-lg">
                        </div>
                        <div class="carousel-item">
                            <img src="https://via.placeholder.com/600x600" alt="Surdo 22'' - Angle 2" class="w-full rounded-lg">
                        </div>
                        <div class="carousel-item">
                            <img src="https://via.placeholder.com/600x600" alt="Surdo 22'' - Angle 3" class="w-full rounded-lg">
                        </div>
                        <div class="flex justify-center mt-4 space-x-2">
                            <button class="carousel-thumbnail w-16 h-16 rounded border-2 border-transparent hover:border-orange-500 overflow-hidden" data-index="0">
                                <img src="https://via.placeholder.com/100x100" alt="Thumbnail 1">
                            </button>
                            <button class="carousel-thumbnail w-16 h-16 rounded border-2 border-transparent hover:border-orange-500 overflow-hidden" data-index="1">
                                <img src="https://via.placeholder.com/100x100" alt="Thumbnail 2">
                            </button>
                            <button class="carousel-thumbnail w-16 h-16 rounded border-2 border-transparent hover:border-orange-500 overflow-hidden" data-index="2">
                                <img src="https://via.placeholder.com/100x100" alt="Thumbnail 3">
                            </button>
                        </div>
                        <button class="carousel-prev absolute left-4 top-1/2 transform -translate-y-1/2 bg-white rounded-full w-10 h-10 flex items-center justify-center shadow-md hover:bg-gray-100">
                            <i class="fas fa-chevron-left text-gray-700"></i>
                        </button>
                        <button class="carousel-next absolute right-4 top-1/2 transform -translate-y-1/2 bg-white rounded-full w-10 h-10 flex items-center justify-center shadow-md hover:bg-gray-100">
                            <i class="fas fa-chevron-right text-gray-700"></i>
                        </button>
                    </div>
                </div>
                
                <div>
                    <h1 class="text-3xl font-bold mb-2">Surdo 22'' - Percusión Brasileña</h1>
                    <div class="flex items-center mb-4">
                        <div class="flex text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                        </div>
                        <span class="text-gray-600">(12 reseñas)</span>
                    </div>
                    
                    <div class="text-2xl font-bold text-orange-600 mb-6">$350.000</div>
                    
                    <p class="text-gray-700 mb-6">
                        El surdo es el corazón de la batería de samba, produciendo los graves profundos que impulsan la música. Nuestro surdo de 22 pulgadas está hecho con madera de alta calidad y pieles naturales para un sonido auténtico.
                    </p>
                    
                    <div class="mb-6">
                        <h3 class="font-bold mb-2">Especificaciones:</h3>
                        <ul class="list-disc pl-5 text-gray-700">
                            <li>Diámetro: 22 pulgadas</li>
                            <li>Altura: 50 cm</li>
                            <li>Material: Madera de jacarandá</li>
                            <li>Piel: Natural de cabra</li>
                            <li>Peso: 5.5 kg</li>
                        </ul>
                    </div>
                    
                    <div class="flex items-center mb-6">
                        <span class="mr-4 font-medium">Cantidad:</span>
                        <div class="flex items-center border rounded-full">
                            <button class="px-3 py-1 text-xl">-</button>
                            <span class="px-4">1</span>
                            <button class="px-3 py-1 text-xl">+</button>
                        </div>
                    </div>
                    
                    <div class="flex space-x-4">
                        <button class="bg-orange-500 text-white px-6 py-3 rounded-full font-medium hover:bg-orange-600 transition flex items-center">
                            <i class="fas fa-shopping-cart mr-2"></i> Añadir al carrito
                        </button>
                        <button class="border-2 border-orange-500 text-orange-500 px-6 py-3 rounded-full font-medium hover:bg-orange-50 transition flex items-center">
                            <i class="far fa-heart mr-2"></i> Guardar
                        </button>
                    </div>
                    
                    <div class="mt-8 pt-6 border-t">
                        <h3 class="font-bold mb-4">También te puede interesar:</h3>
                        <div class="grid grid-cols-3 gap-4">
                            <a href="#" class="text-center">
                                <img src="https://via.placeholder.com/100x100" alt="Related product" class="w-full rounded mb-2">
                                <span class="text-sm">Repinique 12''</span>
                            </a>
                            <a href="#" class="text-center">
                                <img src="https://via.placeholder.com/100x100" alt="Related product" class="w-full rounded mb-2">
                                <span class="text-sm">Caixa 14''</span>
                            </a>
                            <a href="#" class="text-center">
                                <img src="https://via.placeholder.com/100x100" alt="Related product" class="w-full rounded mb-2">
                                <span class="text-sm">Baqueta Surdo</span>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="py-16 bg-orange-50">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <h2 class="text-3xl font-bold mb-6">Sobre Dunun Percusión</h2>
                    <p class="text-gray-700 mb-4">
                        Dunun Percusión nace de la pasión por la música brasileña y el deseo de compartir instrumentos de alta calidad con músicos y grupos de batucada en toda Latinoamérica.
                    </p>
                    <p class="text-gray-700 mb-4">
                        Trabajamos directamente con artesanos brasileños para ofrecer instrumentos auténticos, construidos con materiales de primera calidad y técnicas tradicionales.
                    </p>
                    <p class="text-gray-700 mb-6">
                        Nuestro objetivo es ser el puente entre la rica tradición percusiva de Brasil y los apasionados músicos que buscan llevar ese sonido a sus presentaciones.
                    </p>
                    <a href="#" class="inline-block bg-orange-500 text-white px-6 py-3 rounded-full font-medium hover:bg-orange-600 transition">Conoce nuestra historia</a>
                </div>
                <div class="md:w-1/2">
                    <div class="relative">
                        <img src="https://via.placeholder.com/600x400" alt="Nuestro taller" class="w-full rounded-lg shadow-lg">
                        <div class="absolute -bottom-4 -right-4 bg-white p-4 rounded-lg shadow-lg">
                            <div class="flex items-center">
                                <div class="bg-orange-100 rounded-full h-12 w-12 flex items-center justify-center mr-3">
                                    <i class="fas fa-award text-orange-600 text-xl"></i>
                                </div>
                                <div>
                                    <h4 class="font-bold">Calidad Garantizada</h4>
                                    <p class="text-sm text-gray-600">Instrumentos certificados</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-12">Lo que dicen nuestros clientes</h2>
            
            <div class="grid md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow-sm">
                    <div class="flex items-center mb-4">
                        <div class="flex text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-700 mb-4 italic">
                        "El surdo que compré en Dunun tiene un sonido increíble. La calidad de construcción es excepcional y el servicio al cliente fue excelente."
                    </p>
                    <div class="flex items-center">
                        <img src="https://via.placeholder.com/50x50" alt="Customer" class="rounded-full h-10 w-10 mr-3">
                        <div>
                            <h4 class="font-medium">Carlos M.</h4>
                            <p class="text-sm text-gray-600">Baterista, Samba Tropical</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow-sm">
                    <div class="flex items-center mb-4">
                        <div class="flex text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-700 mb-4 italic">
                        "Hemos equipado a todo nuestro grupo con instrumentos de Dunun. La consistencia en calidad y sonido entre los instrumentos es impresionante."
                    </p>
                    <div class="flex items-center">
                        <img src="https://via.placeholder.com/50x50" alt="Customer" class="rounded-full h-10 w-10 mr-3">
                        <div>
                            <h4 class="font-medium">Ana L.</h4>
                            <p class="text-sm text-gray-600">Directora, Batucada del Sol</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-gray-50 p-6 rounded-lg shadow-sm">
                    <div class="flex items-center mb-4">
                        <div class="flex text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                        </div>
                    </div>
                    <p class="text-gray-700 mb-4 italic">
                        "El servicio postventa es excelente. Cuando necesité ajustar la tensión de mi repinique, me guiaron paso a paso. ¡Muy recomendados!"
                    </p>
                    <div class="flex items-center">
                        <img src="https://via.placeholder.com/50x50" alt="Customer" class="rounded-full h-10 w-10 mr-3">
                        <div>
                            <h4 class="font-medium">Jorge R.</h4>
                            <p class="text-sm text-gray-600">Percusionista independiente</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Instagram Feed -->
    <section class="py-12 bg-gray-100">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center mb-8">
                <h2 class="text-3xl font-bold">Síguenos en Instagram</h2>
                <a href="https://instagram.com/dununpercusion" target="_blank" class="flex items-center text-orange-600 font-medium mt-4 md:mt-0">
                    <i class="fab fa-instagram text-2xl mr-2"></i> @dununpercusion
                </a>
            </div>
            
            <div class="instagram-feed">
                <!-- These would be dynamically loaded from Instagram API -->
                <div class="instagram-item overflow-hidden rounded-lg">
                    <img src="https://via.placeholder.com/300x300" alt="Instagram post" class="w-full h-full object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="instagram-item overflow-hidden rounded-lg">
                    <img src="https://via.placeholder.com/300x300" alt="Instagram post" class="w-full h-full object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="instagram-item overflow-hidden rounded-lg">
                    <img src="https://via.placeholder.com/300x300" alt="Instagram post" class="w-full h-full object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="instagram-item overflow-hidden rounded-lg">
                    <img src="https://via.placeholder.com/300x300" alt="Instagram post" class="w-full h-full object-cover hover:scale-105 transition duration-300">
                </div>
                <div class="instagram-item overflow-hidden rounded-lg">
                    <img src="https://via.placeholder.com/300x300" alt="Instagram post" class="w-full h-full object-cover hover:scale-105 transition duration-300">
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contacto" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <h2 class="text-3xl font-bold mb-6">Contacto</h2>
                    <p class="text-gray-700 mb-6">
                        ¿Tienes preguntas sobre nuestros productos? ¿Necesitas un instrumento personalizado? Contáctanos y te responderemos lo antes posible.
                    </p>
                    
                    <div class="space-y-4">
                        <div class="flex items-start">
                            <div class="bg-orange-100 rounded-full h-10 w-10 flex items-center justify-center mr-4">
                                <i class="fas fa-envelope text-orange-600"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Correo Electrónico</h4>
                                <a href="mailto:ventas@dununpercusion.com" class="text-orange-600 hover:underline">ventas@dununpercusion.com</a>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-orange-100 rounded-full h-10 w-10 flex items-center justify-center mr-4">
                                <i class="fas fa-phone-alt text-orange-600"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Teléfono / WhatsApp</h4>
                                <a href="tel:+573202556865" class="text-orange-600 hover:underline">+57 320 2556865</a>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-orange-100 rounded-full h-10 w-10 flex items-center justify-center mr-4">
                                <i class="fas fa-map-marker-alt text-orange-600"></i>
                            </div>
                            <div>
                                <h4 class="font-medium">Ubicación</h4>
                                <p class="text-gray-700">Bogotá, Colombia</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-8">
                        <h4 class="font-medium mb-4">Síguenos en redes sociales</h4>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-gray-100 h-10 w-10 rounded-full flex items-center justify-center text-gray-700 hover:bg-orange-500 hover:text-white transition">
                                <i class="fab fa-facebook-f"></i>
                            </a>
                            <a href="#" class="bg-gray-100 h-10 w-10 rounded-full flex items-center justify-center text-gray-700 hover:bg-orange-500 hover:text-white transition">
                                <i class="fab fa-instagram"></i>
                            </a>
                            <a href="#" class="bg-gray-100 h-10 w-10 rounded-full flex items-center justify-center text-gray-700 hover:bg-orange-500 hover:text-white transition">
                                <i class="fab fa-youtube"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <div class="bg-gray-50 p-6 rounded-lg shadow-sm">
                        <h3 class="text-xl font-bold mb-4">Envíanos un mensaje</h3>
                        <form>
                            <div class="mb-4">
                                <label for="name" class="block text-gray-700 mb-2">Nombre</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-500">
                            </div>
                            <div class="mb-4">
                                <label for="email" class="block text-gray-700 mb-2">Correo Electrónico</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-500">
                            </div>
                            <div class="mb-4">
                                <label for="subject" class="block text-gray-700 mb-2">Asunto</label>
                                <input type="text" id="subject" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-500">
                            </div>
                            <div class="mb-4">
                                <label for="message" class="block text-gray-700 mb-2">Mensaje</label>
                                <textarea id="message" rows="4" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-500"></textarea>
                            </div>
                            <button type="submit" class="bg-orange-500 text-white px-6 py-3 rounded-full font-medium hover:bg-orange-600 transition w-full">
                                Enviar Mensaje
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter -->
    <section class="py-12 bg-orange-500 text-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl font-bold mb-2">Suscríbete a nuestro boletín</h2>
            <p class="mb-6 max-w-2xl mx-auto">Recibe las últimas novedades, promociones especiales y consejos para el cuidado de tus instrumentos.</p>
            <form class="max-w-md mx-auto flex">
                <input type="email" placeholder="Tu correo electrónico" class="flex-grow px-4 py-3 rounded-l-lg focus:outline-none text-gray-900">
                <button type="submit" class="bg-orange-700 px-6 py-3 rounded-r-lg font-medium hover:bg-orange-800 transition">
                    Suscribirse
                </button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 flex items-center">
                        <img src="https://via.placeholder.com/40x40" alt="Logo" class="h-8 mr-2">
                        Dunun Percusión
                    </h3>
                    <p class="text-gray-400 mb-4">
                        Especialistas en instrumentos de percusión brasileña de alta calidad.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="font-bold text-lg mb-4">Productos</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Surdos</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Repiniques</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Caixas</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Tamborins</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Accesorios</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold text-lg mb-4">Empresa</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Sobre Nosotros</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Talleres</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Blog</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Contacto</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Trabaja con Nosotros</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="font-bold text-lg mb-4">Ayuda</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Preguntas Frecuentes</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Envíos y Devoluciones</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Política de Privacidad</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Términos y Condiciones</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition">Guía de Cuidado</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2023 Dunun Percusión. Todos los derechos reservados.</p>
                <div class="flex space-x-6">
                    <img src="https://via.placeholder.com/50x30" alt="Payment method" class="h-8">
                    <img src="https://via.placeholder.com/50x30" alt="Payment method" class="h-8">
                    <img src="https://via.placeholder.com/50x30" alt="Payment method" class="h-8">
                    <img src="https://via.placeholder.com/50x30" alt="Payment method" class="h-8">
                </div>
            </div>
        </div>
    </footer>

    <!-- Shopping Cart Sidebar -->
    <div class="fixed inset-y-0 right-0 w-full md:w-96 bg-white shadow-lg transform translate-x-full transition duration-300 z-50" id="shopping-cart">
        <div class="h-full flex flex-col">
            <div class="p-4 border-b flex justify-between items-center">
                <h3 class="text-lg font-bold">Tu Carrito (3)</h3>
                <button id="close-cart" class="text-gray-500 hover:text-gray-700">
                    <i class="fas fa-times"></i>
                </button>
            </div>
            
            <div class="flex-grow overflow-y-auto p-4 space-y-4">
                <!-- Cart Item 1 -->
                <div class="flex border-b pb-4">
                    <div class="w-20 h-20 bg-gray-100 rounded overflow-hidden">
                        <img src="https://via.placeholder.com/100x100" alt="Product" class="w-full h-full object-cover">
                    </div>
                    <div class="ml-4 flex-grow">
                        <h4 class="font-medium">Surdo 22''</h4>
                        <p class="text-sm text-gray-500">Percusión brasileña</p>
                        <div class="flex justify-between items-center mt-2">
                            <div class="flex items-center border rounded-full">
                                <button class="px-2 py-1 text-sm">-</button>
                                <span class="px-2 text-sm">1</span>
                                <button class="px-2 py-1 text-sm">+</button>
                            </div>
                            <span class="font-medium">$350.000</span>
                        </div>
                    </div>
                </div>
                
                <!-- Cart Item 2 -->
                <div class="flex border-b pb-4">
                    <div class="w-20 h-20 bg-gray-100 rounded overflow-hidden">
                        <img src="https://via.placeholder.com/100x100" alt="Product" class="w-full h-full object-cover">
                    </div>
                    <div class="ml-4 flex-grow">
                        <h4 class="font-medium">Repinique 12''</h4>
                        <p class="text-sm text-gray-500">Percusión brasileña</p>
                        <div class="flex justify-between items-center mt-2">
                            <div class="flex items-center border rounded-full">
                                <button class="px-2 py-1 text-sm">-</button>
                                <span class="px-2 text-sm">1</span>
                                <button class="px-2 py-1 text-sm">+</button>
                            </div>
                            <span class="font-medium">$280.000</span>
                        </div>
                    </div>
                </div>
                
                <!-- Cart Item 3 -->
                <div class="flex border-b pb-4">
                    <div class="w-20 h-20 bg-gray-100 rounded overflow-hidden">
                        <img src="https://via.placeholder.com/100x100" alt="Product" class="w-full h-full object-cover">
                    </div>
                    <div class="ml-4 flex-grow">
                        <h4 class="font-medium">Baqueta Surdo</h4>
                        <p class="text-sm text-gray-500">Accesorio</p>
                        <div class="flex justify-between items-center mt-2">
                            <div class="flex items-center border rounded-full">
                                <button class="px-2 py-1 text-sm">-</button>
                                <span class="px-2 text-sm">2</span>
                                <button class="px-2 py-1 text-sm">+</button>
                            </div>
                            <span class="font-medium">$45.000</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="p-4 border-t">
                <div class="flex justify-between mb-2">
                    <span>Subtotal</span>
                    <span>$675.000</span>
                </div>
                <div class="flex justify-between mb-4">
                    <span>Envío</span>
                    <span class="text-orange-600">Calculado al pagar</span>
                </div>
                <button class="bg-orange-500 text-white w-full py-3 rounded-full font-medium hover:bg-orange-600 transition">
                    Proceder al Pago
                </button>
                <p class="text-center text-sm text-gray-500 mt-2">o <a href="#" class="text-orange-600 hover:underline">Seguir Comprando</a></p>
            </div>
        </div>
    </div>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Dropdown menus
        document.querySelectorAll('.dropdown').forEach(dropdown => {
            const button = dropdown.querySelector('button');
            const menu = dropdown.querySelector('.dropdown-menu');
            
            button.addEventListener('click', () => {
                menu.classList.toggle('hidden');
            });
        });

        // Shopping cart toggle
        document.querySelectorAll('[href="#"], .fa-shopping-cart').forEach(el => {
            el.addEventListener('click', function(e) {
                if(this.classList.contains('fa-shopping-cart') || this.getAttribute('href') === '#') {
                    e.preventDefault();
                    document.getElementById('shopping-cart').classList.remove('translate-x-full');
                }
            });
        });

        document.getElementById('close-cart').addEventListener('click', function() {
            document.getElementById('shopping-cart').classList.add('translate-x-full');
        });

        // Product carousel functionality
        if(document.querySelector('.carousel')) {
            const carouselItems = document.querySelectorAll('.carousel-item');
            const thumbnails = document.querySelectorAll('.carousel-thumbnail');
            const prevBtn = document.querySelector('.carousel-prev');
            const nextBtn = document.querySelector('.carousel-next');
            let currentIndex = 0;

            function showItem(index) {
                carouselItems.forEach(item => item.classList.remove('active'));
                carouselItems[index].classList.add('active');
                currentIndex = index;
            }

            thumbnails.forEach((thumb, index) => {
                thumb.addEventListener('click', () => showItem(index));
            });

            prevBtn.addEventListener('click', () => {
                let newIndex = currentIndex - 1;
                if(newIndex < 0) newIndex = carouselItems.length - 1;
                showItem(newIndex);
            });

            nextBtn.addEventListener('click', () => {
                let newIndex = currentIndex + 1;
                if(newIndex >= carouselItems.length) newIndex = 0;
                showItem(newIndex);
            });

            // Auto-rotate carousel
            setInterval(() => {
                let newIndex = currentIndex + 1;
                if(newIndex >= carouselItems.length) newIndex = 0;
                showItem(newIndex);
            }, 5000);
        }

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                if(this.getAttribute('href') !== '#') {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
