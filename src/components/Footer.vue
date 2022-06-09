<template>
    <footer>
        <div class="cols container">
            <a class="logo" href="/">
                <img src="../assets/img/la-molisana-logo.png" alt="La molisana" />
            </a>

            <div class="footer-links">
                <h4>Pastificio</h4>
                <nav>
                    <ul>
                        <li><a href="#">Il Pastificio</a></li>
                        <li><a href="#">Grano</a></li>
                        <li><a href="#">Filiera</a></li>
                        <li><a href="#">100 anni di pasta</a></li>
                        <li><a href="#">Sartoria della pasta</a></li>
                    </ul>
                </nav>
            </div>

            <div class="footer-links">
                <h4>Prodotti</h4>
                <nav>
                    <ul>
                        <li><a href="#">Le classiche</a></li>
                        <li><a href="#">Le Integrali</a></li>
                        <li><a href="#">Le Speciali</a></li>
                        <li><a href="#">Le Biologiche</a></li>
                        <li><a href="#">Le Gluten-free</a></li>
                    </ul>
                </nav>
            </div>
        </div>

        <img src="../assets/img/footer-montagne-bottom.jpg" alt="montagne" />
    </footer>
</template>

<script>
export default {
    name: "Footer",
};
</script>

<style scoped lang="scss">
@import "../assets/style/vars";

footer {
    padding-top: 3rem;

    .cols {
        display: flex;
        margin-bottom: 3rem;

        .logo,
        .footer-links {
            flex-basis: calc(100% / 3);
            padding: 0 1rem;
        }

        h4 {
            text-transform: uppercase;
            font-size: 1.25em;
            font-weight: 600;
            margin-bottom: 1rem;
        }

        ul {
            list-style: none;

            li a {
                display: inline-block;
                margin-bottom: 0.25rem;
                text-decoration: none;
                font-size: 0.875em;

                &:hover {
                    color: $primary;
                }
            }
        }
    }
}
</style>