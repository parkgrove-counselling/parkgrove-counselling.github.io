+++
title = "Katie Thompson"
tagline = "Counsellor"
+++

# Welcome

2016x1512 : 758.66 KB 24Bit colour
scales to
640x480
512x384
470x352

h-96 640x384
h-80 640x300


640x300 - desktop max
301x300 - desktop min
640x300 - tablet
593x300 - iphone portrait
301x300 - iphone landscape

640x300
470x300
300x300

the maximum that the div gets is 640

for small pics h-56, h-72 for bigger pics.

2016x1512 : 758.66 KB 24Bit colour

{{ $image := .Resources.Get "images/practice/hillfoot-sofa1.jpg" }}
{{ $image600 := $image.Resize "600x400" }}

<img src="{{ $image600.RelPermalink }}" width="{{ $image.Width }}" height="{{ $image.Height }}">


{{ $imageSofa := resources.Get "images/practice/hillfoot-sofa1.jpg" }}
<!--<img src="{{ $imageSofa.RelPermalink }}" width="{{ $imageSofa.Width }}" height="{{ $imageSofa.Height }}">-->

{{ $image := resources.Get "images/practice/hillfoot-sofa1.jpg" }}
{{ $image640 := $image.Fill "640x300" }}
{{ $image470 := $image.Fill "470x300" }}
{{ $image300 := $image.Fill "300x300" }}

When the break point is 600

iphone se the image div is : 301x288

desktop : 640x288

<!--<img src="{{ $image640.RelPermalink }}" width="{{ $image640.Width }}" height="{{ $image640.Height }}">-->

<!--<img src="{{ $image470.RelPermalink }}" width="{{ $image470.Width }}" height="{{ $image470.Height }}">-->

<!--<img src="{{ $image300.RelPermalink }}" width="{{ $image300.Width }}" height="{{ $image300.Height }}">-->

<!--<hr/>-->

<div id="default-carousel" class="relative w-full" data-carousel="static">
    <!-- Carousel wrapper -->
    <div class="relative h-72 overflow-hidden rounded-lg">
        <!-- Item 1 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <picture>
                <source media="(max-width: 469px)" srcset="{{ $image470.RelPermalink }}" />
                <source media="(min-width: 470px)" srcset="{{ $image640.RelPermalink }}" />
                <img src="{{ $image470.RelPermalink }}" alt="Chris standing up holding his daughter Elva" />
            </picture>
<!--            <img src="{{ $image640.RelPermalink }}" width="{{ $image640.Width }}" height="{{ $image640.Height }}">-->
        </div>
        <!-- Item 2 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <img src="/images/practice/hillfoot-blinds.jpg" class="absolute block w-full -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" loading="lazy" alt="...">
        </div>
        <!-- Item 3 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <img src="/images/practice/hillfoot-clock.jpg" class="absolute block w-full -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" loading="lazy" alt="...">
        </div>
        <!-- Item 4 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <img src="/images/practice/hillfoot-window.jpg" class="absolute block w-full -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" loading="lazy" alt="...">
        </div>
        <!-- Item 5 -->
        <div class="hidden duration-700 ease-in-out" data-carousel-item>
            <img src="/images/practice/hillfoot-single-chair.jpg" class="absolute block w-full -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" loading="lazy" alt="...">
        </div>
    </div>
    <!-- Slider indicators -->
    <div class="absolute z-30 flex -translate-x-1/2 bottom-1 left-1/2 space-x-3 rtl:space-x-reverse">
        <button type="button" class="w-3 h-3 rounded-full" aria-current="true" aria-label="Slide 1" data-carousel-slide-to="0"></button>
        <button type="button" class="w-3 h-3 rounded-full" aria-current="false" aria-label="Slide 2" data-carousel-slide-to="1"></button>
        <button type="button" class="w-3 h-3 rounded-full" aria-current="false" aria-label="Slide 3" data-carousel-slide-to="2"></button>
        <button type="button" class="w-3 h-3 rounded-full" aria-current="false" aria-label="Slide 4" data-carousel-slide-to="3"></button>
        <button type="button" class="w-3 h-3 rounded-full" aria-current="false" aria-label="Slide 5" data-carousel-slide-to="4"></button>
    </div>
    <!-- Slider controls -->
    <button type="button" class="absolute top-0 start-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none" data-carousel-prev>
        <span class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none">
            <svg class="w-4 h-4 text-white dark:text-gray-800 rtl:rotate-180" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 6 10">
                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 1 1 5l4 4"/>
            </svg>
            <span class="sr-only">Previous</span>
        </span>
    </button>
    <button type="button" class="absolute top-0 end-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none" data-carousel-next>
        <span class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none">
            <svg class="w-4 h-4 text-white dark:text-gray-800 rtl:rotate-180" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 6 10">
                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 9 4-4-4-4"/>
            </svg>
            <span class="sr-only">Next</span>
        </span>
    </button>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/flowbite/2.2.1/flowbite.min.js"></script>
