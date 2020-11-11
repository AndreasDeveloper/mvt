<template>
    <div class="dashboard-wrapper">
        <div class="dashboard-wrapper__content">
            <div class="dashboard-wrapper__content__section">
                <h2>Add To Watchlist</h2>
                <div class="add-block" @click="addMovieM = true">
                    <PlusIcon class="add-icon" fill="#000" />
                </div>
            </div>
        </div>
        <AddMovieModal v-if="addMovieM" />
    </div>
</template>

<script>
import PlusIcon from '@/assets/icons/add.svg';
import AddMovieModal from '@/components/dashboard/AddMovieModal';

export default {
    name: 'Dashboard',
    components: {
        PlusIcon,
        AddMovieModal
    },
    data() {
        return {
            addMovieM: false
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/styles/pages/_dashboard.scss';
@import '@/styles/components/_m-blocks.scss';
</style>