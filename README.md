```java
public void btnBackOnAction(ActionEvent actionEvent) throws IOException {
    displayScreen("/view/dashBoard.fxml");
}

void displayScreen(String s) throws IOException {
    Stage stage = (Stage) root.getScene().getWindow();
    stage.setScene(new Scene(FXMLLoader.load(this.getClass().getResource(s))));
    stage.centerOnScreen();
}
```
