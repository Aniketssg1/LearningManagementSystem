<template>
    <div class="header">
        <div class="container-fluid">
            <div id="imageDiv">
                <img id="mkclLogo" src="../assets/MKCL-Logo.svg" class="img-fluid" alt="MKCL logo">
            </div>
            <div id="examNameDiv">
                <h1 class="exam-name">Mid Term Assignment</h1>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style>
.container-fluid {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

#imageDiv {
    display: flex;
    align-items: center;
    position: relative;
}

#mkclLogo {
    width: 100px;
    height: 100px;
    padding: 2px;
    margin-right: 10px;
}

#examNameDiv {
    display: flex;
    align-items: center;
}

.header {
    height: 100px;
    background-color: red;
    background-image: linear-gradient(rgb(255, 196, 0), yellow);
}

.exam-name {
    font-family: 'the-murder';
    src: url('../assets/THE\ MURDER.ttf')
}
</style>
