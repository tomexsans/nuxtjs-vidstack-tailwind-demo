<script setup>
import 'vidstack/styles/defaults.css'
import 'vidstack/styles/community-skin/video.css'

import { defineCustomElements } from 'vidstack/elements';

defineCustomElements();

</script>

<template>
    <div class="flex justify-center items-center min-h-screen md:flex-col">
        <media-player
            class="w-[50%]"
            title="Sprite Fight"
            src="https://stream.mux.com/VZtzUzGRv02OhRnZCxcNg49OilvolTqdnFLEqBsTwaxU/low.mp4"
            poster="https://image.mux.com/VZtzUzGRv02OhRnZCxcNg49OilvolTqdnFLEqBsTwaxU/thumbnail.webp?time=268&width=980"
            thumbnails="https://media-files.vidstack.io/sprite-fight/thumbnails.vtt"
            aspect-ratio="16/9"
            crossorigin
            >
            <media-outlet>
                <media-poster
                alt="Girl walks into sprite gnomes around her friend on a campfire in danger!"
                ></media-poster>
            <track
                src="https://media-files.vidstack.io/sprite-fight/subs/english.vtt"
                label="English"
                srclang="en-US"
                kind="subtitles"
                default
                />
                <track
                src="https://media-files.vidstack.io/sprite-fight/chapters.vtt"
                srclang="en-US"
                kind="chapters"
                default
                />
            </media-outlet>
            <media-community-skin></media-community-skin>
        </media-player>

        <section class="mt-20 text-white">
            <h1 class="text-white text-3xl">Vidstack + NuxtJS + TailWind CSS</h1>
            <p class="mt-5">
                Zero Configuration
            </p>
            <p class="mt-5">
                <a href="#">View More Demo ..</a>
            </p>

            <a href="https://github.com/tomexsans/nuxtjs-vidstack-tailwind-demo">by @tomexsans</a>
        </section>
    </div>
  </template>