<template>
    <div>
        <section>
            <h1 class="mt-8 mb-16 text-4xl font-extrabold leading-none tracking-tight text-gray-900 md:text-5xl lg:text-4xl text-center dark:text-white items">Upcoming Movies</h1>

            <ul class="grid grid-cols-5 gap">
                <li v-for="mov in movies">
                    <MovieCard
                        :poster_path="mov.poster_path"
                        :title="mov.title"
                        :id="mov.id"
                        :overview="mov.overview"
                        :release_date="mov.release_date"
                        :popularity="mov.popularity"
                        :item="mov"
                    />
                </li>
                <br><br>
            </ul>

        </section>

    </div>
</template>

<script setup>
    const movies = useState(() => [])

    const {data} = await useFetch('/api/movies/upcoming',{
        transform: data => {
            movies.value = data.upcomingMovies.results
            
        }
    })
</script>

