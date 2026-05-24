<script lang="ts">
  import { Card, CardContent } from "$lib/components/ui/card";
  import { Badge } from "$lib/components/ui/badge";
  import { Button } from "$lib/components/ui/button";
</script>

<section id="demo" class="py-24 bg-muted/30">
  <div class="container mx-auto px-4 text-center">
    <h2 class="text-sm font-bold uppercase tracking-wider text-muted-foreground mb-12">Trusted by growing restaurants</h2>
    
    <div class="max-w-4xl mx-auto">
      <Card class="overflow-hidden border-border/50 bg-card/60 backdrop-blur-md shadow-lg">
        <CardContent class="p-0">
          <div class="flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 p-8 md:p-12 text-left space-y-6">
              <Badge variant="secondary" class="bg-primary/20 text-primary hover:bg-primary/30 font-semibold border-none">Live Client</Badge>
              <h3 class="font-heading text-3xl font-bold text-foreground">Rangoli Sweets & Chaats</h3>
              <p class="text-muted-foreground leading-relaxed text-lg">
                They make authentic sweets and refreshing drinks using pure milk. They also serve delicious North Indian street food like pani puri and vada pav.
              </p>
              <div class="pt-4">
                <a href="https://rangolisweets.pages.dev/" target="_blank" rel="noopener noreferrer">
                  <Button variant="outline" class="group">
                    View Live Menu 
                    <span class="ml-2 group-hover:translate-x-1 transition-transform">→</span>
                  </Button>
                </a>
              </div>
            </div>
            <div class="md:w-1/2 bg-muted h-full min-h-[350px] w-full relative">
               <div class="absolute inset-0 bg-gradient-to-tr from-primary/20 to-purple-400/20 mix-blend-overlay z-10"></div>
               <img src="https://placehold.co/600x400/171717/00a877?text=Rangoli+Menu" alt="Rangoli Sweets Menu" class="absolute inset-0 w-full h-full object-cover grayscale-[20%] hover:grayscale-0 transition-all duration-500" />
            </div>
          </div>
        </CardContent>
      </Card>
    </div>
  </div>
</section>
