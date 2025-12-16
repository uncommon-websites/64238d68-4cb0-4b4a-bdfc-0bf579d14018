<script>
  const articles = [
    {
      title: "Wealth Management for a New Generation: Wealthfront Goes...",
      author: "Mike Volpi",
      image: "https://images.unsplash.com/photo-1556761175-5973dc0f32e7?q=80&w=600&auto=format&fit=crop"
    },
    {
      title: "Security's Agentic Era Starts Here: Our Investment in 7AI",
      author: "Shardul Shah",
      image: "https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?q=80&w=600&auto=format&fit=crop"
    },
    {
      title: "Getting to know the Bornstein brothers",
      author: "Nina Achadjian",
      image: "https://images.unsplash.com/photo-1519389950473-47ba0277781c?q=80&w=600&auto=format&fit=crop"
    }
  ];
</script>

<section class="py-12 md:py-16 overflow-hidden">
  <div class="container mx-auto px-6 md:px-12 relative">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each articles as article}
        <div class="group cursor-pointer">
          <div class="aspect-[16/10] overflow-hidden mb-6 bg-gray-100">
            <img 
              src={article.image} 
              alt={article.title}
              class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105"
            />
          </div>
          <h3 class="text-xl font-light text-gray-900 mb-3 leading-snug group-hover:text-gray-600 transition-colors">
            {article.title}
          </h3>
          <p class="text-xs text-gray-500 uppercase tracking-wide">by {article.author}</p>
        </div>
      {/each}
    </div>

    <!-- Navigation Arrow -->
    <div class="absolute top-1/2 -right-4 md:right-4 transform -translate-y-1/2 hidden md:block">
      <button class="w-12 h-12 flex items-center justify-center text-gray-400 hover:text-black transition-colors" aria-label="Next">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M9 18L15 12L9 6" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round"/>
        </svg>
      </button>
    </div>
  </div>
</section>
