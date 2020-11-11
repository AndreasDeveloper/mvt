<template>
    <transition name="modal">
        <div class="modal-mask">
            <div class="modal-wrapper add-movie-modal">
                <h2>Add New Movie</h2>
                <form>
                    <input type="text" placeholder="Movie Name" required>
                    <input type="text" placeholder="Movie Description">
                    <button class="add-btn" type="submit">Add</button>
                </form>
            </div>
        </div>
    </transition>
</template>

<script>
export default {
    name: 'AddMovieModal'
}
</script>

<style lang="scss" scoped>
@import '@/styles/components/_modals.scss';
@import '@/styles/components/_buttons.scss';
</style>