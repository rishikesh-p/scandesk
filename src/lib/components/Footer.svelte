<script lang="ts">
  import { Button } from "$lib/components/ui/button";
</script>

<footer id="contact" class="border-t border-border/40 bg-background pt-16 pb-8">
  <div class="container mx-auto px-4 text-center space-y-12">
    <div class="space-y-6 max-w-2xl mx-auto">
      <h2 class="font-heading text-3xl font-bold">Ready to modernize your menu?</h2>
      <p class="text-muted-foreground text-lg">Join forward-thinking restaurants providing a premium digital experience.</p>
      <div class="pt-4 flex flex-col sm:flex-row justify-center items-center gap-4">
        <a href="tel:+916369169287" class="w-full sm:w-auto">
          <Button size="lg" class="w-full text-base font-semibold">
            Call +91 63691 69287
          </Button>
        </a>
        <a href="#pricing" class="w-full sm:w-auto">
          <Button variant="outline" size="lg" class="w-full text-base">Contact Sales</Button>
        </a>
      </div>
    </div>
    
    <div class="border-t border-border/40 pt-8 flex items-center justify-center text-sm text-muted-foreground">
      <p>&copy; {new Date().getFullYear()} ScanDesk. All rights reserved.</p>
    </div>
  </div>
</footer>
