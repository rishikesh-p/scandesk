<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import CircleCheck from "@lucide/svelte/icons/circle-check";
</script>

<section id="pricing" class="py-24">
  <div class="container mx-auto px-4 max-w-4xl text-center space-y-12">
    <div class="space-y-4">
      <h2 class="font-heading text-3xl sm:text-4xl font-bold tracking-tight text-foreground">Simple, transparent pricing</h2>
      <p class="text-lg text-muted-foreground">No hidden fees. Modernize your menu today.</p>
    </div>
    
    <div class="mx-auto max-w-lg rounded-3xl border border-border/50 bg-card p-8 shadow-xl relative overflow-hidden">
      <div class="absolute top-0 right-0 p-6 -mt-4 -mr-4 opacity-10">
        <div class="w-32 h-32 rounded-full bg-primary blur-3xl"></div>
      </div>
      
      <div class="relative z-10 space-y-8">
        <div class="text-left space-y-2">
          <h3 class="text-2xl font-bold font-heading">Digital Menu Plan</h3>
          <div class="flex items-baseline gap-2">
            <span class="text-4xl font-extrabold tracking-tight">₹2000</span>
            <span class="text-muted-foreground">/ starting price</span>
          </div>
        </div>
        
        <ul class="text-left space-y-4">
          <li class="flex items-center gap-3">
             <CircleCheck class="text-primary h-5 w-5 flex-shrink-0" />
             <span class="text-foreground/80">Beautiful Mobile-First Design</span>
          </li>
          <li class="flex items-center gap-3">
             <CircleCheck class="text-primary h-5 w-5 flex-shrink-0" />
             <span class="text-foreground/80">Lightning Fast Loading</span>
          </li>
          <li class="flex items-center gap-3">
             <CircleCheck class="text-primary h-5 w-5 flex-shrink-0" />
             <span class="text-foreground/80">No App Download Required</span>
          </li>
          <li class="flex items-center gap-3">
             <CircleCheck class="text-primary h-5 w-5 flex-shrink-0" />
             <span class="text-foreground/80">Custom QR Code</span>
          </li>
        </ul>
        
        <a href="#contact">
          <Button size="lg" class="w-full text-base font-semibold shadow-lg shadow-primary/20 hover:shadow-primary/40 transition-shadow">
            Get Started Now
          </Button>
        </a>
      </div>
    </div>
  </div>
</section>
