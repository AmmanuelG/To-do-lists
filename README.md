# To-do-lists
a list maker using html css and javascrip


btn.addEventListener('click', function (e) {


    let inpv = input.value

    let newToDO = ''
    const li = document.createElement('li')

    li.classList = 'list'

    li.textContent = inpv

    newToDO = li

    outputUl.append(newToDO)

    console.log(outputUl)

    const btnD = document.createElement('button')

    btnD.classList = 'btn-delete'

    console.log(btnD)
    outputUl.append(btnD)

    const btnE = document.createElement('button'

    btnE.classList = 'btn-edit'

    console.log(btnE)
    outputUl.appendChild(btnE)
    input.value = ''
    // console.log(outputUl, 'with btne')
    btnD.addEventListener('click', function (e) {
        li.remove()
        btnE.remove()
        btnD.remove()

    })
    btnE.addEventListener('click', function (e) {
        input.value = li.textContent
        li.remove()
        btnE.remove()
        btnD.remove()

        li.textContent = input.valued
    })
    e.preventDefault()
})


