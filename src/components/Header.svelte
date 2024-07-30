<script>
    let isNavbarVisible = false;
  
    const toggleNavbar = () => {
      isNavbarVisible = !isNavbarVisible;
    };
  </script>
  
  <body class="bg-gray-300 text-gray-800">
    <header class="bg-white shadow-md ">
        <nav class="container mx-auto px-4 flex items-center justify-between py-4">
            <ul class="flex font-weight:800">
                <li class="font-bold"><a href="#"><img src="favicon.ico" alt="Logo">TakeItAll</a></li>                    
            </ul>
            <div class="relative" x-data="{ isOpen: false }">
                <button @click="isOpen = !isOpen" class="flex items-center" @keydown.escape="isOpen = false" type="button">
                    <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16">
                        <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"/>
                    </svg>
                </button>
                <ul

                    x-show="isOpen"
                    @click.away="isOpen = false"
                    class="absolute font-normal bg-white shadow overflow-hidden rounded w-48 border mt-2 py-1 right-0 z-20">
                    <li>
                        <a href="#" class="flex items-center px-3 py-3 hover:bg-gray-200">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-bag" viewBox="0 0 16 16">
                                <path d="M8 1a2.5 2.5 0 0 1 2.5 2.5V4h-5v-.5A2.5 2.5 0 0 1 8 1m3.5 3v-.5a3.5 3.5 0 1 0-7 0V4H1v10a2 2 0 0 0 2 2h10a2 2 0 0 0 2-2V4zM2 5h12v9a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1z"/>
                            </svg>
                            <span class="ml-2">Cart</span>
                        </a>
                    </li>
                    <li class="">
                        <a href="#" class="flex items-center px-3 py-3 hover:bg-gray-200">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-heart-fill" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M8 1.314C12.438-3.248 23.534 4.735 8 15-7.534 4.736 3.562-3.248 8 1.314"/>
                            </svg>
                            <span class="ml-2">Wishlist</span>
                        </a>
                    </li>
                    <li class="">
                        <a href="#" class="flex items-center px-3 py-3 hover:bg-gray-200">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-in-left" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M10 3.5a.5.5 0 0 0-.5-.5h-8a.5.5 0 0 0-.5.5v9a.5.5 0 0 0 .5.5h8a.5.5 0 0 0 .5-.5v-2a.5.5 0 0 1 1 0v2A1.5 1.5 0 0 1 9.5 14h-8A1.5 1.5 0 0 1 0 12.5v-9A1.5 1.5 0 0 1 1.5 2h8A1.5 1.5 0 0 1 11 3.5v2a.5.5 0 0 1-1 0z"/>
                                <path fill-rule="evenodd" d="M4.146 8.354a.5.5 0 0 1 0-.708l3-3a.5.5 0 1 1 .708.708L5.707 7.5H14.5a.5.5 0 0 1 0 1H5.707l2.147 2.146a.5.5 0 0 1-.708.708z"/>
                            </svg>
                            <span class="ml-2">Login</span>
                        </a>
                    </li>
                </ul>
            </div>
        </nav>
    </header>