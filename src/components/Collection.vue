<template>
    <div id="collection" class="collection">
        <div class="collection-info-wrapper">
            <div class="collection__info collection-info">
                <p class="collection-info__preview">Винтажи коллекций</p>
                <h2 class="collection-info__title title_resize">Март 1980 Урожай Бордо</h2>
                <p class="collection-info__text">
                    У вин насыщенный, изысканный вкус,
                    обладающий хорошей концентрацией фруктовых полутонов,
                    гибкой танинностью и великолепной текстурой.
                    На фоне нюансов дуба выделяются мягкие штрихи вишни и сливы,
                    а долгое послевкусие наполнено пряными намеками.
                </p>
                <table class="collection-info__table collection-info-table">
                    <tbody>
                        <tr class="collection-info-table__row">
                            <td class="collection-info-table__date">1980</td>
                            <td class="collection-info-table__info">
                                <b>Chateau Ducru-Beaucaillou, Saint-Julien AOC 2-eme Grand Cru Classe</b><br>Шато
                                Дюкрю-Бокайю
                            </td>
                        </tr>
                        <tr class="collection-info-table__row">
                            <td class="collection-info-table__date">1988</td>
                            <td class="collection-info-table__info">
                                <b>Вино Chateau Cheval Blanc, St-Emilion AOC 1-er Grand Cru Classe</b><br>Шато Шеваль
                                Блан
                            </td>
                        </tr>
                        <tr class="collection-info-table__row">
                            <td class="collection-info-table__date collection-info-table__date_last">1996</td>
                            <td class="collection-info-table__info collection-info-table__info_last">
                                <b>Chateau Cantemerle, Haut-Medoc AOC 5-me Grand Cru</b><br>Шато Кантмерль
                            </td>
                        </tr>
                    </tbody>
                </table>
                <p class="collection-info__text collection-info__text_last">
                    Вина отлично в сочетании с блюдами из красного мяса,
                    пернатой дичью под красным соусом,
                    рагу из белого мяса под белым соусом,
                    уткой с трюфелем, выдержанными сырами.
                </p>
                <a href="./" class="collection-info__button button_gold">Узнать больше</a>
            </div>
        </div>
        <div class="collection__photo collection-photo">
            <div class="collection-photo-grid">
                <div class="collection-photo__single-wrapper">
                    <img class="collection-photo__big" src="../assets/collection-wine-1.png" alt="бутылки вина">
                </div>

                <div class="collection-photo__multi-wrapper">
                    <img class="collection-photo__small collection-photo__small-1" src="../assets/collection-wine-2.png"
                        alt="бутылки вина">
                    <img class="collection-photo__small collection-photo__small-2" src="../assets/collection-wine-3.png"
                        alt="бутылки вина">
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.collection {
    display: flex;
    border-top: 1px solid #998431;
    border-bottom: 1px solid #998431;
    padding: 60px 0;
}

.collection-info-wrapper {
    flex: 1;
}

.collection-info {
    width: 90%;
}

.collection-info__title {
    line-height: 54px;
    font-weight: 700;
    color: #282828;
    width: 300px;
}

.collection-info__title::after {
    content: "";
    width: 160px;
    height: 1px;
    background-color: #282828;
    display: block;
    margin-top: 30px;
}

.collection-info__text {
    margin: 30px 0;
}

.collection-info__text_last {
    margin-bottom: 40px;
}

.collection-info-table {
    border-collapse: collapse;
}

.collection-info-table__date,
.collection-info-table__info {
    padding: 15px;
    border-bottom: 1px solid #282828;
}

.collection-info-table__date_last,
.collection-info-table__info_last {
    border-bottom: none;
}

.collection-info-table__date {
    border-right: 1px solid #282828;
}

.collection-info-table__info b {
    font-size: 18px;
    font-family: 'Playfair Display', sans-serif;
}

.collection-info__button {
    margin-top: 10px;
}

.collection__photo {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.collection-photo-grid {
    display: flex;
    flex-direction: column;
}

.collection-photo__multi-wrapper {
    display: flex;
    justify-content: space-between;
    margin-top: 22px;
}

.collection-photo__big {
    width: 100%;
}

.collection-photo__small {
    width: calc(50% - 15px);
}

.collection-photo__small-1 {
    margin-right: 30px;
}

@media screen and (max-width: 1439px) {
    .collection-info {
        width: auto;
    }

    .collection__photo {
        justify-content: start;
    }

    .collection-photo__single-wrapper {
        display: flex;
        justify-content: center;
    }

    .collection-photo__multi-wrapper {
        flex-direction: column;
        align-items: center;
    }

    .collection-photo__big {
        width: 70%;
    }

    .collection-photo__small {
        width: 70%;
    }

    .collection-photo__small-1 {
        margin-right: 0;
        margin-bottom: 30px;
    }
}

@media screen and (max-width: 1249px) {
    .collection {
        flex-direction: column;
    }

    .collection-info-table {
        width: 100%;
    }

    .collection-photo-grid {
        flex-direction: row;
        margin-top: 45px;
    }

    .collection-photo__single-wrapper {
        display: none;
    }

    .collection-photo__multi-wrapper {
        margin-top: 0;
        flex-direction: row;
        flex: 3;
    }

    .collection-photo__small {
        width: calc(50% - 15px);
    }

    .collection-photo__small-1 {
        margin: 0;
        margin-right: 15px;
    }

    .collection-photo__single-wrapper {
        justify-content: center;
        flex: 2;
    }
}

@media screen and (max-width: 768px) {
    .collection {
        padding: 30px 0;
    }

    .collection-info__title::after {
        margin-top: 15px;
    }

    .collection-info__text {
        margin: 18px 0;
    }

    .collection-info__text_last {
        margin-bottom: 40px;
    }
}

@media screen and (max-width: 592px) {
    .collection-photo__multi-wrapper {
        flex-direction: column;
        align-items: flex-start;
    }

    .collection-photo__small {
        width: auto;
    }

    .collection-photo__small-1 {
        margin: 0;
        margin-bottom: 25px;
    }
}

@media screen and (max-width: 330px) {
    .collection-info__title {
        width: auto;
    }
}
</style>