<script>
    import Header from './Header.svelte'
    import Box from './Box.svelte'

    let items = [
        {
            "title": "How to rock, Part 1",
            "author": "wayne",
            "create_date": new Date(Date.UTC(2023, 1, 17, 12, 33)),
            "body": "In short, Svelte is a way of writing user interface components — like a navigation bar, comment section, or contact form — that users see and interact with in their browsers. The Svelte compiler converts your components to JavaScript that can be run to render the HTML for the page and to CSS that styles the page. You don't need to know Svelte to understand the rest of this guide, but it will help. "
        },
        {
            "title": "Rocking while keeping your socks on",
            "author": "garth",
            "create_date": new Date(Date.UTC(2023, 1, 17, 12, 33)),
            "body": "In short, Svelte is a way of writing user interface components — like a navigation bar, comment section, or contact form — that users see and interact with in their browsers. The Svelte compiler converts your components to JavaScript that can be run to render the HTML for the page and to CSS that styles the page. You don't need to know Svelte to understand the rest of this guide, but it will help. "
        },
        {
            "title": "The Adventure Ahead",
            "author": "bill",
            "create_date": new Date(Date.UTC(2023, 1, 17, 12, 33)),
            "body": "In short, Svelte is a way of writing user interface components — like a navigation bar, comment section, or contact form — that users see and interact with in their browsers. The Svelte compiler converts your components to JavaScript that can be run to render the HTML for the page and to CSS that styles the page. You don't need to know Svelte to understand the rest of this guide, but it will help. "
        },
        {
            "title": "Oh no, not again",
            "author": "ted",
            "create_date": new Date(Date.UTC(2023, 1, 17, 12, 33)),
            "body": "In short, Svelte is a way of writing user interface components — like a navigation bar, comment section, or contact form — that users see and interact with in their browsers. The Svelte compiler converts your components to JavaScript that can be run to render the HTML for the page and to CSS that styles the page. You don't need to know Svelte to understand the rest of this guide, but it will help. "
        }
    ];
</script>

<div class="lg:flex flex-grow items-center">
{#each items as item}
    <Box { item }/>
{/each}
</div>
