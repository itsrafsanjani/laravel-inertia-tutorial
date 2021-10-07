<template>
    <h1 class="text-4xl">Users</h1>

    <Nav />

    <div style="margin-top: 600px">
        <p>Current time is {{ time }}</p>

        <Link href="/users" class="text-blue-500" preserve-scroll>
            Refresh
        </Link>
    </div>
</template>

<script>
import Nav from "../Shared/Nav";
import { Link } from "@inertiajs/inertia-vue3";
export default {
    components: {
        Nav,
        Link
    },
    props: {
        time: String
    }
};
</script>
