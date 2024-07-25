var tabsLabels = document.querySelectorAll('.tabs__label')
tabsLabels.forEach(function(tabLabelActive) {
  tabLabelActive.addEventListener('click', function() {
    tabsLabels.forEach(function(tabLabelTheRest) {
      tabLabelTheRest.classList.remove('active')
    })
    tabLabelActive.classList.add('active')
  })
})