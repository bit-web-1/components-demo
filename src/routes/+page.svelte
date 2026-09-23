<script>
    import billm from '$lib/assets/images/groundhog-day.webp';
</script>

<header>
    <h1>SvelteKit Components Demonstration</h1>
    <p>For more information, view the <a href="https://svelte.dew/tutorial">Svelte tutorial</a></p>
    <nav>
        <a href="/">Home</a>
    </nav>
</header>

<main>
    <article class="card">
        <img src="{billm}" alt="Phil Connors">
        <section>
            <h2>Phill Connors</h2>
            <dl>
                <dt>Favourite song:</dt>
                <dd>I Got You Babe</dd>
                <dt>Pet's name:</dt>
                <dd>Punxsutawney Phil</dd>
            </dl>
        </section>
    </article>
</main>

<footer>
    <p>ID512 Fundamentals of Web Development &copy; 1993</p>
</footer>

<style>
    :global(body) {
        margin: 0;
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    }

    header {
        background-color: #f8f8f8;
        padding: 1rem;
        border-bottom: 1px solid #ccc;
        nav {
            border-top: 1px solid #ccc;
            margin-top: 1rem;
            padding-top: 1rem;
        }
    }

    footer {
        background-color: #f8f8f8;
        padding: 1rem;
        border-top: 1px solid #ccc;
        text-align: center;
    }

    .card {
        img {
            width: 200px;
            aspect-ratio: 1 / 1;
            object-fit: cover;
            object-position: center;
            border-radius: 30px;
            corner-shape: squircle;
        }
        display: flex;
        align-items: center;
        gap: 2rem;
        border: 1px solid #ccc;
        border-radius: 5px;
        padding: 1rem;
        max-width: 600px;
        margin: 1rem;
    }

    dl {
        display: grid;
        grid-template-columns: max-content 1fr;
        gap: 0.5rem 1rem;
    }

    dt {
        font-weight: bold;
    }

    dd {
        margin: 0;
    }
</style>