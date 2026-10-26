I had a problem with test_module.py and pandas functioning with a newer version.
##  THE ERROR GIVEN
class DataCleaningTestCase(unittest.TestCase):
    def test_data_cleaning(self):
        actual = int(time_series_visualizer.df.count(numeric_only=True))
        expected = 1238
        self.assertEqual(actual, expected, "Expected DataFrame count after cleaning to be 1238.")

You can see in my print(df.shape[0]), that the actual shape of the DF is equal to the one expected after the cleaning
