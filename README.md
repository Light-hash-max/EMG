# EMG
# Вот какие требования у клиента:
# 1. При запуске программы мы видим 3D пространство с неровной земной поверхностью (подложкой) и
простым интерфейсом.
# 2. Подложка в зависимости от высоты окрашена в разные цвета по произвольной гипсометрической
шкале.
# 3. Для перемещения и вращения камеры используется правая кнопка мыши (ПКМ). Нажатие и
удерживание ПКМ - перемещение «хватанием» за пол (как в google картах). Shift+ПКМ - вращение
камеры вокруг точки, на которую смотрит камера. Ни при каких условиях камера не должна уходить
под землю.
# 4. При нажатии на кнопку &quot;создать плашку&quot; в интерфейсе мы переходим в режим создания плашек. Если
в этом режиме кликнуть левой кнопкой мыши (ЛКМ) по полу, то над ним создается плашка, после чего
режим создания отключается и сразу открывается интерфейс редактирования текста новой плашки.
Появление созданной плашки должно быть с анимацией (придумайте сами).
# 5. При нажатии ЛКМ на созданную плашку, она выделяется и появляется окно интерфейса, в котором
можно изменить текст у выделенной плашки. При изменении текста, размеры плашки подстраиваются
под размеры текста. Появление и исчезновение интерфейса редактирования должно быть
анимировано (придумайте сами как).
# 6. Если мы НЕ в режиме &quot;создать плашку&quot;, то клик ЛКМ в пустоту/пол снимает выделение с плашек.
# 7. Выделив плашку и удерживая ЛКМ, плашку можно перетаскивать. Если удерживать ALT меняется
высота расположения плашки над землей, иначе плашка перемещается параллельно плоскости пола.
Плашка никогда не должна опускаться ниже уровня поверхности земли или поднимается выше некого
заданного уровня делающего плашку никогда не видимой для камеры.
# 8. Также необходимо реализовать возможность выделять и снимать выделение с нескольких плашек с
использованием клавиши CTRL, с возможностью группового редактирования/удаления/перемещения
выделенных плашек.
# 9. При нажатии кнопки Delete выделенные плашки удаляются.
# 10. * Вместо кнопки и режима создания плашки в интерфейсе сделать UI иконку плашки, которую
с помощью Drag&amp;Drop ЛКМ можно перетащить на подложку, тем самым создав в месте
броска новую плашку и вызвав интерфейс ее изменения.

# 11. * Добавить в интерфейс слайдер &quot;Изолинии&quot;. Когда этот слайдер равен 0 подложка
отображается как сплошная карта, когда он сдвигается подложка начинает отображаться как
Изолинии с шагом указанным в качестве параметра этого слайдера.
# 12. * Добавить в интерфейс кнопку &quot;Землетрясение&quot; при нажатии на которую подложка начинает
анимировано, случайным образом менять свою высоту и окраску. Все плашки считаются
привязанными к высоте над уровнем земли и если земля под плашкой поднимается плашка
поднимается на ту же высоту.
# 13. * Добавить кнопку &quot;Трубопровод&quot;. При нажатии на нее на подложке берутся 2 случайные
точки наблюдаемые из камеры. Необходимо сгенерировать геометрию выходящую из под
земли в одной точке, идущую по изгибам поверхности до другой точки и там уходящую под
землю. Желательно сделать эту геометрию похожей на трубопровод (материалом, текстурой,
дополнительными деталями или подпорками).
