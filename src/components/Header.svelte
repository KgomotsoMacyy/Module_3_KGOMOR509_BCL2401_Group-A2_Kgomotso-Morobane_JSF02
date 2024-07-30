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
            <div class="relative">
                <button class="flex items-center" @keydown.escape="isOpen = false" type="button">
                    <svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16">
                        <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5"/>
                    </svg>
                </button>
            </div>
        </nav>
    </header>
  </body>