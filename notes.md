(function(module) {
  var articlesController = {};

  // DONE: Create the `articles` table when the controller first loads, with
  //       code that was previously in index.html.
  // DONE: Make the function below fetch and render the articles. It should look
  //       very similiar to code you wrote before.
  // DONE: Hide the main section elements; reveal the #articles section:
  articlesController.index = function() {
    Article.createTable();
    Article.fetchAll(articleView.initIndexPage);
    $('.tab-content').hide();
    $('#articles').show();
  };

  module.articlesController = articlesController;
})(window);

Example of FP.
