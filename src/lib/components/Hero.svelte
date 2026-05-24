<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import heroMockup from "$lib/assets/hero_mockup.png";
</script>

<section class="relative overflow-hidden py-20 lg:py-32">
  <div class="container mx-auto px-4 flex flex-col lg:flex-row items-center gap-12">
    <div class="flex-1 text-center lg:text-left space-y-8">
      <h1 class="font-heading text-5xl sm:text-6xl lg:text-7xl font-extrabold tracking-tight text-foreground leading-[1.1]">
        People buy with their <span class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-purple-400">eyes first.</span>
      </h1>
      <p class="text-2xl text-foreground/90 font-medium leading-relaxed max-w-2xl mx-auto lg:mx-0">
        Turn your menu into a powerful sales machine.
      </p>
      <p class="text-lg text-muted-foreground leading-relaxed max-w-2xl mx-auto lg:mx-0">
        Why let customers scroll through plain text menus when you can make them crave every dish visually? ScanDesk's lightning-fast, mobile-first QR menus wow your customers and increase sales. No app download required.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-4">
        <a href="#demo"><Button size="lg" class="w-full sm:w-auto text-base">View Live Demo</Button></a>
        <a href="#contact"><Button size="lg" variant="outline" class="w-full sm:w-auto text-base">Contact Sales</Button></a>
      </div>
    </div>
    
    <div class="flex-1 w-full max-w-[400px] lg:max-w-none relative mx-auto">
      <div class="hero-mockup relative rounded-3xl border border-border/50 bg-card p-2 shadow-2xl overflow-hidden transition-transform duration-500">
        <img 
          src={heroMockup} 
          alt="ScanDesk Mobile Menu Demo" 
          class="rounded-2xl w-full h-auto object-cover border border-border/20"
        />
        <div class="absolute inset-0 bg-gradient-to-t from-background/80 to-transparent pointer-events-none rounded-3xl"></div>
      </div>
      <!-- Ambient glow -->
      <div class="absolute -inset-x-20 -inset-y-20 z-[-1] bg-primary/20 blur-[100px] rounded-full opacity-50"></div>
    </div>
  </div>
</section>

<style>
  .hero-mockup {
    transform: perspective(1000px) rotateY(-6deg) rotateX(3deg);
  }
  .hero-mockup:hover {
    transform: perspective(1000px) rotateY(0deg) rotateX(0deg);
  }

  @media (max-width: 768px) {
    .hero-mockup {
      transform: none;
    }
  }
</style>
