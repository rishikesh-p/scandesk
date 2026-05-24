<script lang="ts">
  import { Button } from "$lib/components/ui/button";
  import Menu from "@lucide/svelte/icons/menu";
  import X from "@lucide/svelte/icons/x";
  import Sun from "@lucide/svelte/icons/sun";
  import Moon from "@lucide/svelte/icons/moon";
  import logo from "$lib/assets/logo.png";
  import { toggleMode } from "mode-watcher";

  let mobileMenuOpen = $state(false);

  function toggleMenu() {
    mobileMenuOpen = !mobileMenuOpen;
  }

  function closeMenu() {
    mobileMenuOpen = false;
  }
</script>

<header class="sticky top-0 z-50 w-full border-b border-border/40 bg-background/95 backdrop-blur supports-[backdrop-filter]:bg-background/60">
  <div class="container mx-auto px-4 h-16 flex items-center justify-between">
    <!-- Logo -->
    <a href="/" class="flex items-center space-x-2">
      <img src={logo} alt="ScanDesk Logo" class="h-8 w-auto" />
      <span class="font-heading font-bold text-2xl tracking-tight text-primary">ScanDesk</span>
    </a>

    <!-- Desktop Nav -->
    <nav class="hidden md:flex items-center space-x-6 text-sm font-medium" aria-label="Main navigation">
      <a href="#features" class="transition-colors hover:text-foreground/80 text-foreground/60">Features</a>
      <a href="#demo" class="transition-colors hover:text-foreground/80 text-foreground/60">Demo</a>
      <a href="#pricing" class="transition-colors hover:text-foreground/80 text-foreground/60">Pricing</a>
      <a href="#contact" class="transition-colors hover:text-foreground/80 text-foreground/60">Contact</a>
    </nav>

    <!-- Mobile Menu Button -->
    <div class="md:hidden flex items-center space-x-2">
      <Button variant="ghost" size="icon" onclick={toggleMode} class="h-9 w-9">
        <Sun class="h-5 w-5 dark:hidden" />
        <Moon class="hidden h-5 w-5 dark:block" />
        <span class="sr-only">Toggle theme</span>
      </Button>
      <Button variant="ghost" size="icon" onclick={() => mobileMenuOpen = !mobileMenuOpen} aria-label="Toggle menu">
        {#if mobileMenuOpen}
          <X class="h-6 w-6" />
        {:else}
          <Menu class="h-6 w-6" />
        {/if}
      </Button>
    </div>

    <!-- Desktop CTA -->
    <div class="hidden md:flex items-center space-x-4">
      <Button variant="ghost" size="icon" onclick={toggleMode} class="h-9 w-9">
        <Sun class="h-5 w-5 dark:hidden" />
        <Moon class="hidden h-5 w-5 dark:block" />
        <span class="sr-only">Toggle theme</span>
      </Button>
      <a href="#contact">
        <Button>Get Started</Button>
      </a>
    </div>


  </div>

  <!-- Mobile Menu -->
  {#if mobileMenuOpen}
    <div class="md:hidden border-t border-border/40 bg-background/98 backdrop-blur-lg animate-in slide-in-from-top-2 duration-200">
      <nav class="container mx-auto px-4 py-4 flex flex-col space-y-3" aria-label="Mobile navigation">
        <a href="#features" onclick={closeMenu} class="py-2 text-sm font-medium text-foreground/70 hover:text-foreground transition-colors">Features</a>
        <a href="#demo" onclick={closeMenu} class="py-2 text-sm font-medium text-foreground/70 hover:text-foreground transition-colors">Demo</a>
        <a href="#pricing" onclick={closeMenu} class="py-2 text-sm font-medium text-foreground/70 hover:text-foreground transition-colors">Pricing</a>
        <a href="#contact" onclick={closeMenu} class="py-2 text-sm font-medium text-foreground/70 hover:text-foreground transition-colors">Contact</a>
        <div class="pt-2 flex flex-col space-y-2 border-t border-border/40">
          <a href="#contact" onclick={closeMenu}>
            <Button class="w-full justify-center">Get Started</Button>
          </a>
        </div>
      </nav>
    </div>
  {/if}
</header>
