<script lang="ts">
  import { Card, CardContent, CardHeader, CardTitle, CardDescription } from "$lib/components/ui/card";
  import Zap from "@lucide/svelte/icons/zap";
  import Palette from "@lucide/svelte/icons/palette";
  import QrCode from "@lucide/svelte/icons/qr-code";
  import Smartphone from "@lucide/svelte/icons/smartphone";
</script>

<section id="features" class="py-24 relative">
  <div class="absolute inset-0 bg-background/50 -z-10"></div>
  <div class="container mx-auto px-4">
    <div class="text-center space-y-4 mb-16">
      <h2 class="font-heading text-3xl sm:text-4xl font-bold tracking-tight text-foreground">Why choose ScanDesk?</h2>
      <p class="text-lg text-muted-foreground max-w-2xl mx-auto">Everything you need to modernize your dining experience.</p>
    </div>
    
    <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
      <Card class="bg-card/50 backdrop-blur-sm hover:bg-muted/50 transition-all border-border/50 hover:border-primary/50 shadow-sm hover:shadow-md group">
        <CardHeader>
          <div class="h-12 w-12 rounded-xl bg-primary/10 flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <Zap class="text-primary" size={24} />
          </div>
          <CardTitle>Blazing Fast</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription class="text-base text-muted-foreground">Instant loads, optimized images (WebP), and zero lag for a seamless browsing experience.</CardDescription>
        </CardContent>
      </Card>
      
      <Card class="bg-card/50 backdrop-blur-sm hover:bg-muted/50 transition-all border-border/50 hover:border-primary/50 shadow-sm hover:shadow-md group">
        <CardHeader>
          <div class="h-12 w-12 rounded-xl bg-primary/10 flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <Palette class="text-primary" size={24} />
          </div>
          <CardTitle>Premium Design</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription class="text-base text-muted-foreground">Stop using boring PDFs. Give customers a beautiful, interactive browsing experience that drives sales.</CardDescription>
        </CardContent>
      </Card>
      
      <Card class="bg-card/50 backdrop-blur-sm hover:bg-muted/50 transition-all border-border/50 hover:border-primary/50 shadow-sm hover:shadow-md group">
        <CardHeader>
          <div class="h-12 w-12 rounded-xl bg-primary/10 flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <QrCode class="text-primary" size={24} />
          </div>
          <CardTitle>Tabletop QR Codes</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription class="text-base text-muted-foreground">Place a beautiful QR code on every table. Customers simply scan it with their camera to instantly view your menu.</CardDescription>
        </CardContent>
      </Card>
      
      <Card class="bg-card/50 backdrop-blur-sm hover:bg-muted/50 transition-all border-border/50 hover:border-primary/50 shadow-sm hover:shadow-md group">
        <CardHeader>
          <div class="h-12 w-12 rounded-xl bg-primary/10 flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <Smartphone class="text-primary" size={24} />
          </div>
          <CardTitle>No App Required</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription class="text-base text-muted-foreground">Works seamlessly on any smartphone browser. There are no apps to download and no complicated sign-ups.</CardDescription>
        </CardContent>
      </Card>
    </div>
  </div>
</section>
